Users

PKUserId NVARCHAR(10)
FirstName NVARCHAR(50)
LastName NVARCHAR(50)
BirthDate DATE
Email NVARCHAR(100)
Gender NVARCHAR(6)
City NVARCHAR(25)
Country NVARCHAR(25)
Zipcode NVARCHAR(10)
FacebookID NVARCHAR(10)
FacebookToken NVARCHAR(300)
Latitude FLOAT
Longitude FLOAT
AccountStatus BOOLEAN
RegistrationDateTime DATE




Peek

PKPeekId NVARCHAR(10)
PeekName NVARCHAR(50)
Address NVARCHAR(100)
City NVARCHAR(25)
Country NVARCHAR(25)
Zipcode NVARCHAR(10)
Latitude FLOAT
Longitude FLOAT
PeekType NVARCHAR(25)
PeekStatus BOOLEAN
PeekCreationDateTime DATE

xUserPeek

PKUserPeekId NVARCHAR(10)
FKPeekId NVARCHAR(10)
FKUserId NVARCHAR(10)
PeekStatus BOOLEAN
PeekAddDateTime DATE



Post

PKPostId NVARCHAR(10)
FKPeekId NVARCHAR(10)
FKUserId NVARCHAR(10)
Post NVARCHAR(200)
Latitude FLOAT
Longitude FLOAT
PeekStatus BOOLEAN
PostDateTime DATE


xReplies
PKReplyId NVARCHAR(10)
FKPostId NVARCHAR(10)
FKUserId NVARCHAR(10)
Reply NVARCHAR(200)
Latitude FLOAT
Longitude FLOAT
ReplyStatus BOOLEAN
ReplyDateTime DATE




xPostUpvote

PKUpVoteId NVARCHAR(10)
FKPostId NVARCHAR(10)
FKUserId NVARCHAR(10)
Latitude FLOAT
Longitude FLOAT
VoteDateTime DATE


xPostDownVote

PKDownVoteId NVARCHAR(10)
FKPostId NVARCHAR(10)
FKUserId NVARCHAR(10)
Latitude FLOAT
Longitude FLOAT
VoteDateTime DATE


xReplyUpvote

PKUpVoteId NVARCHAR(10)
FKPostId NVARCHAR(10)
FKReplyId NVARCHAR(10)
FKUserId NVARCHAR(10)
Latitude FLOAT
Longitude FLOAT
VoteDateTime DATE


xReplyDownVote
PKDownVoteId NVARCHAR(10)
FKPostId NVARCHAR(10)
FKReplyId NVARCHAR(10)
FKUserId NVARCHAR(10)
Latitude FLOAT
Longitude FLOAT
VoteDateTime DATE




Score
PKScoreId
FKUserId
Score
UpdateDateTime DATE



http://aspspider.ws/rajukhabiya/
