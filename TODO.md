# Tapüy Bride — To Do Before Launch

## SECURITY — Do before sharing with real users
- [ ] Re-enable Row Level Security on all Supabase tables
- [ ] Test that each bride can only see her own data
- [ ] Set up Resend for real email delivery (password resets)
- [ ] Set Supabase Site URL to production domain

## RLS tables to re-enable:
profiles, tasks, budget_items, guests, vendors, 
saved_vendors, forum_threads, forum_replies, wins,
squad_members, squad_messages, squad_polls, photos

## Command to re-enable (run in Supabase SQL Editor):
alter table public.profiles enable row level security;
alter table public.tasks enable row level security;
alter table public.budget_items enable row level security;
alter table public.guests enable row level security;
alter table public.vendors enable row level security;
alter table public.forum_threads enable row level security;
alter table public.forum_replies enable row level security;
alter table public.wins enable row level security;
alter table public.squad_members enable row level security;
alter table public.squad_messages enable row level security;
alter table public.squad_polls enable row level security;
alter table public.photos enable row level security;
