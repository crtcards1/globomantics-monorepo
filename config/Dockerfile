FROM alpine:3.19

# Simulate secrets accidentally baked into a container during build

ENV AWS_ACCESS_KEY_ID=AKIAIOSFODNN7EXAMPLE
ENV AWS_SECRET_ACCESS_KEY=wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY

ENV GITHUB_TOKEN=ghp_abcdefghijklmnopqrstuvwxyz1234567890ABCDE
ENV STRIPE_API_KEY=sk_live_51HGLOBOMANTICSSECRETKEY

# Common mistake: echoing secrets during build
RUN echo "SENDGRID_API_KEY=SG.xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx" > /tmp/secrets.env

CMD ["sleep", "infinity"]
