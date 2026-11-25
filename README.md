# Serverless PDF Converter - Google Cloud

## Overview

An educational cloud computing project demonstrating an
event driven, serverless document to PDF conversion pipeline
using Google Cloud Platform.

## Technologies

- Google Cloud Run
- Google Cloud Storage
- Google Cloud Pub/Sub
- Google Cloud Build
- Identity and Access Management (IAM)
- Docker
- Node.js
- LibreOffice

## Architecture

1. A document is uploaded to a Cloud Storage bucket
2. An object finalization event generates a Pub/Sub message (Event trigger)
3. Pub/Sub delivers an authenticated request to Cloud Run
4. The containerized application converts the document to PDF
5. The generated PDF is stored in an output bucket

## Implementation

- Configured and deployed containerized serverless services
- Configured IAM permissions and authenticated communication
- Troubleshot deployment and document conversion failures
- Adjusted memory, concurrency, and acknowledgment settings
- Validated document conversion functionality

## Documentation

The `docs` directory contains the project proposal,
hands on implementation walkthrough, and presentation link

## Acknowledgments

This academic project is based on Google Cloud Skills Boost
lab GSP644: Build a Serverless App with Cloud Run that
Creates PDF Files.

This repository documents the implementation, configuration,
testing, and troubleshooting process for educational purposes.
