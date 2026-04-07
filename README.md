# simple-sms-client

## Overview

`simple-sms-client` is a minimal SMPP client example written in Python using Twisted. It demonstrates how to connect to an SMPP server, authenticate, and submit a basic SMS message.

## Requirements

- Twisted
- smpp.pdu
- chardet==2.2.1

## Configuration

Connection settings are defined in `settings.py`:

- `HOST` — SMPP server host
- `PORT` — SMPP server port
- `SYSTEM_ID` — SMPP system ID
- `PASSWORD` — SMPP password

## Project Structure

- `app.py` — application entry point
- `smpp_client_factory.py` — Twisted client factory
- `smpp_client_protocol.py` — SMPP protocol implementation
- `settings.py` — connection configuration

## Notes

The protocol implementation includes example authentication and message submission logic. The included example sends a test SMS message after a successful connection. These methods can be modified to support additional SMPP commands.
