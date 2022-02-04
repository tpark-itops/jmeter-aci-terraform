FROM mcr.microsoft.com/azure-cli 

# Install Terraform v1.1.5
RUN wget https://releases.hashicorp.com/terraform/1.1.5/terraform_1.1.5_linux_amd64.zip
RUN unzip terraform_1.1.5_linux_amd64.zip && rm terraform_1.1.5_linux_amd64.zip
RUN mv terraform /usr/bin/terraform

# Install azcopy
RUN wget https://aka.ms/downloadazcopy-v10-linux 
RUN tar -xvf downloadazcopy-v10-linux
RUN mv ./azcopy_linux_amd64_*/azcopy /usr/bin/azcopy
RUN rm -rf downloadazcopy-v10-linux
RUN rm -rf ./azcopy_linux_amd64_*

CMD sh
