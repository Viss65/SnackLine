# SnackLine

A mobile-friendly web prototype for pre-ordering snacks at the USTP CDO canteen. Made for **CS212 – Human-Computer Interaction** (User-Centered Design project), Section CS2B.

**Live prototype:** https://Viss65.github.io/SnackLine/

## The problem
Students buying snacks at the canteen, especially in the afternoon, line up in the same narrow walkway where other students pass through. This causes congestion, uses up limited break time, and discourages reserved students from buying at all.

## What SnackLine does
- Shows 5 real canteen stalls with their menus and prices: thebreadhub, RCFS Fruits Stand, K & I, Vals Food Hub, and Roy's Café
- Shows how busy each stall is (Light, Moderate, Packed) with an estimated wait
- Lets the student add items and choose how much cash they will hand over, so the vendor can prepare the exact change
- Gives a queue number so the student can wait anywhere, not in the walkway
- Shows the order status (Received, Preparing, Ready) and the number of orders ahead
- Gives alerts with sound, vibration, and an on-screen message: "New order received" for the vendor and "Your order is ready!" for the student
- Has a Vendor view to update the order status

## How to run
**Online:** open the live link above on any phone or laptop.

**Locally:** download `index.html` and open it in a browser. No installation needed.

## How to try it

### Option 1: One device
1. Tap **Start ordering**, choose a stall, and add items.
2. Choose the cash amount and tap **Place order**. You get a queue number.
3. Tap the **Vendor** tab, find the order, and tap **Start preparing**, then **Mark ready**.
4. Go back to the **Student** tab to see "Your order is ready!"

### Option 2: Two devices (student phone and vendor device)
The vendor code is **`SNACK26`**.
1. **Vendor device:** tap **Vendor**, then **Start as main vendor device**. Keep this tab open.
2. **Student phone:** tap **Start ordering**. In the card at the top, type the code `SNACK26` and tap **Connect**. It shows "Connected".
3. The student places an order. The vendor device shows "New order received".
4. On the vendor device, tap **Start preparing** and **Mark ready**. The student phone shows "Your order is ready!"
5. Another device can type the same code in the Vendor tab and tap **Join** to log in as a vendor.

Both devices need internet for the two-device connection. If it does not connect, the app still works on one device.

To start fresh for a new tester, use **Reset demo data** in the Vendor tab.

## Implemented vs proposed
| Feature | Status |
| --- | --- |
| Real stalls, menus, and prices | Implemented |
| Crowd indicator per stall | Implemented |
| Cart, cash amount, and change | Implemented |
| Queue number, orders ahead, order status | Implemented |
| Ready and new-order alerts (sound, vibration, on-screen) | Implemented |
| Vendor controls and cancel order | Implemented |
| Order data saved on the device | Implemented |
| Two-device connection using a code | Implemented |
| Sample demo orders for the crowd level | Simulated |
| Vendor side played by a group member during testing | Simulated |
| Real payment (for example GCash) | Proposed |
| SMS or push notifications when the app is closed | Proposed |
| A permanent online server | Proposed |
| Vendor login accounts, real-time stock, order history | Proposed |

## Limitations
- The two-device connection needs internet and uses a free public connection server, so it may not work on every network.
- The main vendor tab must stay open.
- Alerts work while the page is open.
- Crowd level is based only on active orders in the app, not on the real number of people.
- Not yet tested with real canteen staff.

## Built with
HTML, CSS, JavaScript, and PeerJS for the device connection, hosted on GitHub Pages.

## Team
- Elvis R. Belongilot Jr. – Documenter
- Kent Aljon Apuya – Leader
- Earl Justine Ortega – Technical Builder
- Trisha Mae Gala – Designer
