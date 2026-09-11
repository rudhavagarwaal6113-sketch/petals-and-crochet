# Petals & Crochet

A handmade crochet storefront for Chandigarh, backed by Supabase.

## Included
- Supabase Auth customer accounts
- Live products from `public.products`
- Cart and checkout
- Orders + order items in Supabase
- Admin-only product dashboard
- Admin image uploads to `product-images`
- Admin order status management
- ₹599 free-gift threshold
- ₹49 delivery and ₹50 discount on ₹1000+ orders
- Razorpay checkout hooks through Supabase Edge Functions

## Final launch steps
1. Import this GitHub repository into Vercel as a static site.
2. In Supabase Edge Function secrets, add `RAZORPAY_KEY_ID` and `RAZORPAY_KEY_SECRET` from the Razorpay dashboard.
3. Test a small Razorpay payment in test mode first.
4. Switch to live Razorpay keys only after the merchant account is approved.

The frontend only contains the public Supabase URL/key. Never put the Razorpay secret in `script.js`.
