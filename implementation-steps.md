# Implementation Steps

## 1. Created Custom VPC
- CIDR: 10.0.0.0/16

## 2. Created Public Subnet
- CIDR: 10.0.1.0/24

## 3. Created Private Subnet
- CIDR: 10.0.2.0/24

## 4. Attached Internet Gateway
- Configured internet access for public subnet

## 5. Configured Route Tables
- Public subnet routed to Internet Gateway
- Private subnet isolated

## 6. Created Security Groups
### Public SG
- HTTP 80
- HTTPS 443
- TCP 3000

### Private SG
- MySQL 3306 only from public-sg

## 7. Implemented Zero Trust Principles
- Removed SSH access
- Used AWS Systems Manager (SSM)

## 8. Enabled CloudTrail
- Centralized audit logging
- Monitoring of management events

## 9. Result
Successfully implemented a secure Zero Trust cloud architecture on AWS.
