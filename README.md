# TryingVegetta
Trying Vegetta performance testing framework

## Vegetta script examples

uuid=$(uuidgen); echo "GET http://webcache.domain.com/fetch?url=http%3A%2F%2Fdoom.import.io%2Fphp%2Fcrawler-treadmills%2Fpage.php%3Frow%3D56414245%26depth%3D%26encoding%3Dutf-8%26bigMode%3D%26requiresJS%3D%26cacheBust=""$uuid""%3D&ttl=0" | vegeta attack -rate=30 -duration=30s | vegeta report

This should serve as a GET example!

### POST
vegeta attack -targets=target.txt -rate=200 -duration=20s | vegeta report

Using target.txt as target, and body-performance.json as body!
