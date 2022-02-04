FROM alpine 
RUN apk add py3-pip
RUN apk add gcc musl-dev python3-dev libffi-dev openssl-dev cargo make
RUN pip install --upgrade pip
RUN pip install azure-cli
RUN wget https://releases.hashicorp.com/terraform/1.1.5/terraform_1.1.5_linux_amd64.zip
RUN unzip terraform_1.1.5_linux_amd64.zip && rm terraform_1.1.5_linux_amd64.zip
RUN mv terraform /usr/bin/terraform

CMD sh
