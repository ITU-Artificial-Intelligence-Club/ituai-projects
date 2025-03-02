# Mail Service

We have a simple system called mailo, which helps us store user data from different events, with their names, emails and which events they attended.

This system requires a mail service to send emails to users, but ITU's own mailing service only lets us send only 200 emails per day.

Using a provider like Gmail also fails because sending mass emails at the same time is seen as spam.

We need to figure out a new provider, or a way to create our own system to send our emails.

If there is a generic limit to send emails in every provider, like so if you need to send more than 1000, you send 300 every hour or day, we need to figure this out.

This project is not decided how to be implemented yet, so the tech stack is not finalized.

[Mailo Repository](https://github.com/ITU-Artificial-Intelligence-Club/mailo)

## Project Plan

As per the principle of [Occam's Razor](https://en.wikipedia.org/wiki/Occam%27s_razor), our first choice should be the simplest one. That is, using available bulk email solutions. We should resort to hosting our own SMTP server if and ony if it is needed.

1. Investigate available bulk email providers/solutions. [See here](#using-a-ready-email-service)
2. ***IF none are fit for our use case***, investigate hosting our own email server. [See here](#hosting-our-own-email-server)

### Using a Ready Email Service

- Amazon SES (:star: look at this first! :star:)
- Mailgun
- SendGrid
- Postmark

These are just some of the many available email solutions on the internet. If you can find ones better than the ones listed above, please check them out as well.

To properly investigate a solution, one should go through the below checklist and note them down.

**Solution Checklist**
- [ ] Are there any limits? We need around >=1000 mail/day.
- [ ] Is there a free tier? And is it enough for us? 
- [ ] If no free tier, is the service cheap?
- [ ] Which protocols/APIs does it support (e.g. SMTP)? Can it be integrated with our other services/projects?
- [ ] Can the club email (`ituaiclub@itu.edu.tr`) be used? 
- [ ] Are there any rate limits that might affect us? E.g. we are limited to sending only 100 emails in one hour.
- [ ] Is there a chance of our emails going to spam? How can it be avoided?
- [ ] How easy is it to set up and use?
- [ ] Are there any security related considerations?

#### A Working Solution!

We have found a ready email solution that we can use, great! :rocket: :star:

**Now we need to do the following:**

1. Test out on a scratch/temporary email with low-volume and high-volume emails.
2. Do a setup from scratch and note down the process, from start to finish, for other club members.
  - How to use it, how to set up an account...
3. Try integrating it with our other services (if applicable).

If we have done all the steps above, an applause to us! :clap: :confetti:

### Hosting Our Own Email Server

**Possible Options**

- Postfix
- Exim
- Haraka

Again, this is not a comprehensive list. We should research well and choose the best possible technology for our purposes.

To properly investigate a solution, one should go through the below checklist and note them down.

**Solution Checklist**
- [ ] Where and how do we host it? Can we use our current VPS?
- [ ] Can the club email (`ituaiclub@itu.edu.tr`) be used? 
- [ ] Is there a chance of our emails going to spam? How can it be avoided?
- [ ] How easy is it to set up and use?
- [ ] What is the maintanance cost? What do we have to do to keep the server running without error?
- [ ] Are there any security related considerations?
