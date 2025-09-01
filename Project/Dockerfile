FROM  alpine:3.22.1
RUN apk update
RUN apk add python3
RUN apk add py3-pip
WORKDIR /Project
COPY requirements.txt .
# COPY XXXX.py .
#COPY test_XXX.py .
RUN python3 -m venv Projectenv
ENV PATH="/Project/Projectenv/bin:$PATH"
RUN pip install -r requirements.txt
# CMD ["python3", "orders-server.py"]