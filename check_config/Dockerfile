FROM %%BASE_IMAGE%%

# Add env
ENV LANG C.UTF-8

# Setup base
RUN apk add --no-cache tzdata jq python3 \
    && pip3 install --no-cache --upgrade pip

# Copy data
COPY run.sh /
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
