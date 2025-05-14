# MLOps Projects Implementation Plan

## Overview

This document outlines the implementation plan for three MLOps projects using pre-trained models and free tier resources across different cloud platforms. Each project will be implemented, documented, and then brought offline.

---

## Project 1: Real-time Satellite Tracker (GCP)

### Project Scope
A web application that tracks and displays satellites in real-time on an interactive globe using orbital prediction models.

### Free Data Sources
- Space-Track.org API (registration required, free)
- CelesTrak TLE data (public domain)
- NASA Satellite Situation Center API

### Pre-trained Models
- SGP4/SDP4 orbital propagation models
- Pre-trained orbit prediction models

### Implementation Focus
1. **Data Pipeline:**
   - Scheduled data fetching for TLE data
   - Efficient orbital calculations with minimal compute
   - Optimized storage for positioning data

2. **Model Deployment:**
   - Lightweight orbital prediction serving
   - Client-side prediction for interpolation

3. **MLOps Monitoring & Governance:**
   - Request tracking and latency monitoring
   - Execution logs and performance metrics
   - Access control and security policies

4. **User Interface:**
   - Interactive globe visualization
   - Real-time satellite tracking
   - Client-side rendering for performance

### Offline Transition Plan
- Export prediction libraries for local use
- Document API specifications
- Package as standalone application

---

## Project 2: News Clustering with Explainability (Azure)

### Project Scope
An application that clusters news articles from the past 7 days, identifies trends, and provides responsible AI explanations for clustering decisions.

### Free Data Sources
- GDELT Project API
- NewsAPI.org (limited free tier)
- Media Cloud API (academic/non-commercial use)

### Pre-trained Models
- BERT/RoBERTa for text embeddings
- Pre-trained sentence transformers
- Hugging Face transformers for NLP tasks

### Implementation Focus
1. **Data Collection:**
   - Scheduled news article fetching
   - Text extraction and preprocessing
   - Metadata enrichment and storage

2. **Model Deployment:**
   - Transformer-based embedding generation
   - Dynamic clustering algorithms
   - Explainability layer integration

3. **Responsible AI Features:**
   - Bias detection in clustering results
   - Confidence scores for cluster assignments
   - Interpretability dashboards
   - Source diversity metrics

4. **MLOps Governance:**
   - Performance tracking for endpoints
   - Feature attribution monitoring
   - Audit logging for compliance
   - Responsible AI documentation

### Offline Transition Plan
- Export models in ONNX format
- Document model configurations
- Package as standalone application

---

## Project 3: Green Screen Editor App (AWS)

### Project Scope
An application that removes backgrounds from images and videos, allowing users to replace backgrounds with custom images or videos.

### Pre-trained Models
- DeepLabV3+ for semantic segmentation
- U^2-Net for salient object detection
- MODNet for portrait matting
- Background Matting V2 for video processing

### Implementation Focus
1. **Media Processing Pipeline:**
   - Efficient temporary storage
   - Streamlined preprocessing workflow
   - Optimized composition and rendering

2. **Model Optimization:**
   - Model compression techniques
   - Quantization for faster inference
   - Memory usage optimization

3. **Performance Strategies:**
   - Smart image resizing
   - Selective frame processing for videos
   - Result caching and progressive loading

4. **MLOps Monitoring:**
   - Latency and error tracking
   - Performance dashboards
   - Input validation systems
   - Content governance policies

### Offline Transition Plan
- Export optimized models in ONNX format
- Document the processing pipeline
- Package as standalone application

---

## Timeline & Resource Management

### Development Sequence
1. **Month 1:** Azure News Clustering Project
   - Utilize Azure free credits within 30-day window
   - Complete implementation and documentation
   - Export to offline environment

2. **Month 2-3:** AWS Green Screen Editor
   - Implement during first months of free tier
   - Focus on optimization for resource constraints
   - Export to offline environment

3. **Month 3-12:** GCP Satellite Tracker
   - Implement using free tier resources
   - Can extend development as resources allow
   - Export to offline environment

### Documentation Requirements
For each project, document:
1. Architecture diagrams
2. API specifications
3. Model details and performance metrics
4. Configuration templates
5. Monitoring setup
6. Offline deployment instructions

### MLOps Best Practices Applied
- Version control for all code
- Deployment automation
- Model performance tracking
- Responsible AI documentation
- Security controls
- Resource optimization
