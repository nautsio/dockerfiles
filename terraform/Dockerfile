FROM uzyexe/terraform:latest

ADD terraformrc /root/.terraformrc
ADD https://github.com/bennycornelissen/terraform-provider-localfile/releases/download/v0.1/terraform-provider-localfile-linux-amd64 /bin/terraform-provider-localfile
RUN chmod +x /bin/terraform-provider-localfile

