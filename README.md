# Connetz: A Social Networking App

Connetz is a social networking app designed for individuals to publicly showcase their skills and portfolios, engage in discussions, chat with others, and monetize their expertise. It aims to foster collaboration and communication among users from diverse backgrounds. 

## App Evaluation

- **Category:** Social Networking
- **Story:** Connetz allows users to promote their talents and portfolios within their professional fields. Users can engage in public discussions, chat with others, share content, and monetize their skills through posts.
- **Market:** This app is designed for everyone, catering to a wide user base and enabling collaboration and communication among individuals from diverse backgrounds.
- **Habit:** Users can use the app at their convenience, whether they are seeking services, events, or organizational opportunities.
- **Scope:** Connetz has planned phases for its development:
  1. Phase one focuses on skill posting and portfolio showcasing.
  2. Phase two targets larger organizations, likely introducing features tailored for their needs.
  3. Phase three caters to individuals seeking specific services, potentially incorporating features for service requests and fulfillment.

![processed-B9DA4F67-6BF4-436B-933B-BEC8482696EC](https://github.com/FreeFormFAMU/.github/assets/96313489/496c3cb1-ce0c-4a27-bbd3-08a64b89aeca)


https://github.com/FreeFormFAMU/.Konnetz/assets/96313489/aff47ce5-a77e-40ee-84e9-63429eebfd78





## Schema


## Models

## User
| Property | Type | Description |
|-----------------|-----------------|-----------------|
| user_id | Reference | userId Reference |
| username  | String | users unique username |
| email | String | User email | 
| password | String | User password  |
| created_at | TimeStamp | User TimeStamp of created Post |
| updated_at | TimeStamp | User TimeStamp of updated Post |

## Skills
| Property | Type | Description |
|-----------------|-----------------|-----------------|
| skils_id  | Reference | skills_id Reference |
| user_id | Int | user_id Reference |
| skills_name | String | Users skills name |
| skills_description | String | Users skills description |
| created_at | Timestamp | Date value|
| updated_at | Timestamp | Date value |

## Post 
| Property | Type | Description |
|-----------------|-----------------|-----------------|
| post_id | Reference | post_id Refrenece |
| user_id | int | Cloud References |
| content | String | Content information |
| created_at | Timestamp | Date value |
| updated_at | Timestamp | Date value |

## Messages
| Property | Type | Description |
|-----------------|-----------------|-----------------|
| message_id | Reference | message_id Reference |
| sender_id | int | sender_id Reference |
| receiver_id | int | recevicer_id Reference | 
| message_content | String | message content | 
| send_at | Timmestamp | Date value | 
| read_at | Timestamp | Date value | 

## Following
| Property | Type | Description |
|-----------------|-----------------|-----------------|
| following_id | Refernece | following_id Refernece |
| user_id | int | user_id Reference |
| following_user_id | int | following_user_id Reference |

## Followers
| Property | Type | Description |
|-----------------|-----------------|-----------------|
| followers_id | Reference | followers_id Reference |
| user_id | int | Reference |
| follower_user_id | int | Reference |

## Saved Post Table 
| Property | Type | Description |
|-----------------|-----------------|-----------------|
| saved_post_id | Reference | saved_post_id Reference |
| user_id | int | user_id Reference |
| post_id | int | post_id Reference |
| saved_at | Timestamp | Date Value |

## Liked Posts Table 
| Property | Type | Description |
|-----------------|-----------------|-----------------|
| liked_post_id | Reference | liked_post_id Reference |
| user_id | int | user_id Reference |
| post_id | int | post_id Refernece |
| liked_at | Timestamp | Date value |

## Comments Table 
| Property | Type | Description |
|-----------------|-----------------|-----------------|
| comment_id | Reference | comment_id Reference |
| user_id | int | user_id Reference |
| post_id | int | post_id Reference |
| comment_text | String | comment_text string value |
| commented_at | Timestamp | Date value |

## Feed Table 
| Property | Type | Description |
|-----------------|-----------------|-----------------|
| feed_id | Reference | feed_id Reference |
| user_id | int | Reference |
| item_type | string | item_type value |
| item_content | Refernce | photos,videos |
| created_at | Timestamp | Date Value |
| likes_count | int | like_count int value |
| comments_count | int | comments_count int value |


# Networking

Home Screen Feed

  (Read/GET)Query posts randomly based off of saved posts

  (Create/POST) Create a new save on a post

  (Delete) Delete existing save

Create Post Screen

  (Create/POST) Create a new post object

Profile Screen

  (Read/Get) Query logged in user object

  (Update/PUT) Update user profile image

  (Update/PUT) Update user account information









