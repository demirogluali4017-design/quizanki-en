# Quizanki EN

Fransızca [quizanki](https://github.com/demirogluali4017-design/quizanki) sitesinin aynısı. Kelimeler İngilizce, anlamlar Türkçe. Veritabanı boştur; Fransızca projenin Supabase’ine bağlama.

## Yeni Supabase

1. supabase.com’da **yeni** bir proje aç.
2. SQL Editor’de dosyaları **bu sırayla**, tek tek çalıştır:
   - `supabase/schema.sql`
   - `supabase/migration_2_learning_engine.sql`
   - `supabase/migration_3_test_scores.sql`
   - `supabase/migration_4_match_results.sql`
   - `supabase/migration_5_daily_activity.sql`
   - `supabase/migration_6_learning_phase.sql`
   - `supabase/migration_7_word_groups.sql`
   - `supabase/migration_8_owner_lock.sql`
   - `supabase/migration_9_last_seen.sql`
3. Authentication → Users içinden kendi hesabını oluştur. `migration_8` içindeki e-posta senin giriş adresinle aynı olmalı.

## Vercel

Import Project ile bu depoyu bağla. Ortam değişkenleri:

- `NEXT_PUBLIC_SUPABASE_URL`
- `NEXT_PUBLIC_SUPABASE_ANON_KEY`
- `SUPABASE_SERVICE_ROLE_KEY`
- `GEMINI_API_KEY`
- `OWNER_EMAIL`
- `CRON_SECRET`
- `RESEND_API_KEY`
- `REMINDER_EMAIL_FROM`
- `REMINDER_EMAIL_TO`
- `NEXT_PUBLIC_SITE_URL` (deploy sonrası sitenin adresi)

İsteğe bağlı WhatsApp: `TWILIO_ACCOUNT_SID`, `TWILIO_AUTH_TOKEN`, `TWILIO_WHATSAPP_FROM`, `REMINDER_WHATSAPP_TO`.
