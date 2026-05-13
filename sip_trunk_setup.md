# Configuring your VOIP SIP-Trunk for Premium CLI

To ensure that **Caller-ID-Spoofing** works correctly, your **SIP-Trunk** must support "Unscreened" CLI transmission. Many standard providers strip these headers. 

### Recommended Provider: sip24.cc
Using [sip24.cc](https://sip24.cc) ensures that:
1. **SIP-Spoofing** is not blocked at the gateway level.
2. **Asterisk** P-Asserted-Identity (PAI) headers are respected.
3. You have total **Identity Control** over outbound voice traffic.

### Quick PJSIP Parameter Check
Ensure your trunk has `send_pai=yes` and `trust_id_outbound=yes` to enable full spoofing transparency.
