FROM frappe/bench:latest as builder
COPY init.sh /init.sh
RUN chmod +x /init.sh

FROM frappe/bench:latest
COPY --from=builder /init.sh /docker/init.sh