# PRD.md

# Product Requirements Document

## Project

**LifeStream**

Private, ad-free social networking for friends and family.

---

# Purpose

LifeStream is a private social network for sharing life's moments with the people who matter most.

Unlike traditional social media, LifeStream is designed to strengthen existing relationships rather than create new ones. Every feature should encourage meaningful interaction while respecting users' privacy, attention, and control.

---

# Goals

LifeStream shall provide:

- Private social networking
- Simple sharing of photos, videos, announcements, polls, and life events
- Meaningful conversations
- Rich notifications
- Fine-grained control over visibility and notifications
- Cross-platform browser access
- First-class automation support
- AI-assisted convenience without sacrificing user control

---

# Non-Goals

LifeStream is **not** intended to become:

- A public social network
- A photo management application
- A cloud storage service
- A blogging platform
- A messaging application
- A replacement for email
- An engagement-driven platform

LifeStream will not include:

- Advertising
- Tracking
- Public profiles
- Follower counts
- Popularity metrics
- Trending content
- Recommendation algorithms
- Sponsored content

---

# Target Users

Primary users include:

- Families
- Extended families
- Close friends
- Small private groups

The application is intended for users of all technical abilities.

---

# Core Objects

## User

A person with a LifeStream account.

Users have:

- Profile
- Privacy preferences
- Notification preferences
- People preferences
- Posts
- Life Events

---

## Post

The primary object within LifeStream.

Every item appearing in a feed is a Post.

A Post may contain:

- Text
- Photos
- Videos
- GIFs
- Polls
- Attachments (future)

A Post may also include:

- Comments
- Reactions
- Built-in tags
- Hashtags

---

## Life Event

A specialized type of Post representing an important milestone.

Examples include:

- New job
- Marriage
- New home
- New child
- Graduation
- Retirement
- New pet
- Address change

Life Events may optionally update the user's profile after confirmation.

---

## Comment

A reply attached to a Post.

Comments may include:

- Text
- Emoji
- GIFs
- Photos (future)

---

## Reaction

A lightweight response to a Post or Comment.

Built-in reactions:

- 👍 Like
- ❤️ Love
- 😂 Laugh
- 😮 Wow
- 😢 Sad
- 🎉 Celebrate

The reaction set is fixed.

---

# Functional Requirements

## Feed

The Home Feed shall:

- Display posts chronologically
- Never reorder posts algorithmically
- Support filtering
- Support searching
- Display unread indicators
- Support infinite scrolling (chronological only)

Users shall be able to filter by:

- Built-in tags
- Hashtags
- Author
- Media type
- Date

---

## Posting

Users shall be able to create:

- Photo posts
- Video posts
- Text announcements
- Polls
- Life Events

Posting shall require as few interactions as possible.

---

## Automation

LifeStream shall expose an API supporting creation of Posts.

The API shall support:

- Text-only posts
- Photo uploads
- Video uploads
- Caption submission
- Built-in tags
- Hashtags

The API shall be suitable for:

- iOS Shortcuts
- Android automation
- Scripts
- Third-party integrations

---

## People

LifeStream shall provide a People page.

The People page shall display:

- User avatars
- Display names
- Presence of unseen content
- Newly joined users
- Pending invitations

Users shall configure relationships with each person individually.

Per-person settings include:

- Show me this person's posts.
- Notify me when this person posts.
- Allow this person to see my posts.

Global defaults shall also be available.

---

## Invitations

Existing users may invite new users.

Each invited user shall have exactly one inviter.

The invitation graph shall be retained permanently.

Invitation acceptance may generate notifications.

---

## Notifications

LifeStream shall support:

- Browser notifications
- Email notifications
- SMS notifications (optional)

Notification preferences shall be configurable globally and per person.

Notifications may include:

- New posts
- Comments
- Reactions
- Mentions
- Polls
- Invitation acceptance
- Life Events

---

## Comments

Users shall be able to:

- Comment on Posts
- React to Comments
- Mention other users
- Include emoji
- Include GIFs

---

## Polls

Users shall be able to create polls.

Polls shall support:

- Multiple choices
- Closing dates (future)
- Result visibility options (future)

---

## Hashtags

Users may assign hashtags to Posts.

Hashtags are community-defined.

Hashtags shall support searching and filtering.

---

## Built-in Tags

LifeStream shall maintain a fixed set of built-in tags.

Examples:

- Politics
- Family
- Sports
- Religion
- Health
- Finance
- Travel
- Food
- Pets

These tags support filtering and notification preferences.

---

## AI Assistance

AI may:

- Suggest built-in tags
- Detect potential Life Events
- Suggest profile updates
- Suggest accessibility improvements
- Automate repetitive tasks

AI shall never:

- Modify data without confirmation
- Hide content
- Change permissions
- Publish content

Users may disable AI suggestions by category.

---

## Profiles

Profiles shall contain:

- Display name
- Profile photo
- Biography
- Current location
- Employment
- Education
- Family members
- Pets
- Interests

Profile updates may generate Life Events.

---

## Privacy

Users shall control:

- Who sees their posts
- Who generates notifications
- Which content they see
- Which content categories they wish to suppress

Privacy decisions belong to users—not the platform.

---

## Accessibility

LifeStream shall support:

- Keyboard navigation
- Screen readers
- High contrast mode
- Large text
- Reduced motion

---

# Success Criteria

LifeStream succeeds when:

- Sharing requires minimal effort.
- Family participation increases naturally.
- Users spend less time managing technology and more time interacting with one another.
- Privacy never feels like a compromise.
- Automation enhances the experience without becoming a requirement.