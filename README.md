# Autonomous Field Service Orchestrator – Knowledge Base

## FAQs

### How are technicians assigned?
Technicians are assigned based on skills, proximity, and availability using AI-powered optimization.

### What happens if a technician is delayed?
The orchestrator detects the delay using GPS and traffic data, reassigns the job automatically, and notifies the customer.

### How are customers informed?
Customers receive automatic SMS/Email/WhatsApp notifications for scheduling, delays, or rescheduling.

---

## Company Policies

- **SLA Targets:**
  - High Priority: 4 hours
  - Medium Priority: 24 hours
  - Low Priority: 48 hours

- **Customer Notification Policy:**
  Notify customers of any delay or rescheduling at least 30 minutes in advance.

- **Technician Workload:**
  No technician can be assigned more than 5 jobs per day.

---

## SOP – Handling a Service Request

1. Receive request from CRM or API.
2. Extract location, skills required, and priority.
3. Assign technician optimally.
4. Notify both technician and customer.
5. Monitor progress via GPS.
6. If disruption occurs, reassign automatically.

---

## SOP – Handling Delays

1. Detect delay from GPS.
2. If delay > 15 minutes:
   - Reassign to the nearest available technician.
   - Notify customer and new technician.
3. Log the incident for future learning.

---

## References

- [Google Maps Traffic API](https://developers.google.com/maps/documentation/routes)
- [Twilio SMS API](https://www.twilio.com/docs/sms)
