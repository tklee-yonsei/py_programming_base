FROM python:3.14-slim

# 시스템 패키지 업데이트 및 필수 도구 설치
RUN apt-get update && apt-get install -y \
    git \
    curl \
    && rm -rf /var/lib/apt/lists/*

# pip 업그레이드 및 기본 개발 도구 설치
RUN pip install --no-cache-dir --upgrade pip \
    && pip install --no-cache-dir \
    black \
    pylint \
    pytest

# 작업 디렉토리 설정
WORKDIR /workspaces

