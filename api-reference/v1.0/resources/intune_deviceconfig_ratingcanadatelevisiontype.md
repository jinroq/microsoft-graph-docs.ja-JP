# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="9ddf2-101">ratingCanadaTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9ddf2-101">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="9ddf2-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ddf2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ddf2-103">カナダのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="9ddf2-103">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="9ddf2-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="9ddf2-104">Members</span></span>
|<span data-ttu-id="9ddf2-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="9ddf2-105">Member</span></span>|<span data-ttu-id="9ddf2-106">値</span><span class="sxs-lookup"><span data-stu-id="9ddf2-106">Value</span></span>|<span data-ttu-id="9ddf2-107">説明</span><span class="sxs-lookup"><span data-stu-id="9ddf2-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ddf2-108">allAllowed</span><span class="sxs-lookup"><span data-stu-id="9ddf2-108">allAllowed</span></span>|<span data-ttu-id="9ddf2-109">0</span><span class="sxs-lookup"><span data-stu-id="9ddf2-109">0%</span></span>|<span data-ttu-id="9ddf2-110">既定値、すべてのテレビ番組コンテンツを許可</span><span class="sxs-lookup"><span data-stu-id="9ddf2-110">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="9ddf2-111">allBlocked</span><span class="sxs-lookup"><span data-stu-id="9ddf2-111">allBlocked</span></span>|<span data-ttu-id="9ddf2-112">1</span><span class="sxs-lookup"><span data-stu-id="9ddf2-112">-1</span></span>|<span data-ttu-id="9ddf2-113">すべてのテレビ番組コンテンツを不許可</span><span class="sxs-lookup"><span data-stu-id="9ddf2-113">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="9ddf2-114">子</span><span class="sxs-lookup"><span data-stu-id="9ddf2-114">children</span></span>|<span data-ttu-id="9ddf2-115">2</span><span class="sxs-lookup"><span data-stu-id="9ddf2-115">-2</span></span>|<span data-ttu-id="9ddf2-116">C 区分は 2 歳から 7 歳の子供に適しています</span><span class="sxs-lookup"><span data-stu-id="9ddf2-116">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="9ddf2-117">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="9ddf2-117">childrenAbove8</span></span>|<span data-ttu-id="9ddf2-118">3</span><span class="sxs-lookup"><span data-stu-id="9ddf2-118">"3"</span></span>|<span data-ttu-id="9ddf2-119">C8 区分は 8 歳以上の子供に適しています</span><span class="sxs-lookup"><span data-stu-id="9ddf2-119">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="9ddf2-120">general</span><span class="sxs-lookup"><span data-stu-id="9ddf2-120">General</span></span>|<span data-ttu-id="9ddf2-121">4</span><span class="sxs-lookup"><span data-stu-id="9ddf2-121">-4</span></span>|<span data-ttu-id="9ddf2-122">G 区分は一般視聴者に適しています</span><span class="sxs-lookup"><span data-stu-id="9ddf2-122">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="9ddf2-123">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="9ddf2-123">parentalGuidance</span></span>|<span data-ttu-id="9ddf2-124">5</span><span class="sxs-lookup"><span data-stu-id="9ddf2-124">.5</span></span>|<span data-ttu-id="9ddf2-125">PG、保護者による助言と指導が必要です</span><span class="sxs-lookup"><span data-stu-id="9ddf2-125">PG, Parental Guidance</span></span>|
|<span data-ttu-id="9ddf2-126">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="9ddf2-126">agesAbove14</span></span>|<span data-ttu-id="9ddf2-127">6</span><span class="sxs-lookup"><span data-stu-id="9ddf2-127">-6</span></span>|<span data-ttu-id="9ddf2-128">14+ 区分は 14 歳以上の視聴者が対象です</span><span class="sxs-lookup"><span data-stu-id="9ddf2-128">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="9ddf2-129">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="9ddf2-129">agesAbove18</span></span>|<span data-ttu-id="9ddf2-130">7</span><span class="sxs-lookup"><span data-stu-id="9ddf2-130">-7</span></span>|<span data-ttu-id="9ddf2-131">18+ 区分は 18 歳 以上の視聴者が対象です</span><span class="sxs-lookup"><span data-stu-id="9ddf2-131">The 18+ classification is intended for viewers ages 18 and older</span></span>|








