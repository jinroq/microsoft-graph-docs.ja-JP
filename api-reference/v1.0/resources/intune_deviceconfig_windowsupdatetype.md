# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="c9f05-101">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c9f05-101">windowsUpdateType enum type</span></span>

> <span data-ttu-id="c9f05-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c9f05-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9f05-103">分岐デバイスから更新を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="c9f05-103">Determines which branch devices will receive their updates from Possible values are: , , .</span></span>
## <a name="members"></a><span data-ttu-id="c9f05-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="c9f05-104">Members</span></span>
|<span data-ttu-id="c9f05-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="c9f05-105">Member</span></span>|<span data-ttu-id="c9f05-106">値</span><span class="sxs-lookup"><span data-stu-id="c9f05-106">Value</span></span>|<span data-ttu-id="c9f05-107">説明</span><span class="sxs-lookup"><span data-stu-id="c9f05-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9f05-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="c9f05-108">UserDefined</span></span>|<span data-ttu-id="c9f05-109">0</span><span class="sxs-lookup"><span data-stu-id="c9f05-109">0%</span></span>|<span data-ttu-id="c9f05-110">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="c9f05-110">Allow the user to set.</span></span>|
|<span data-ttu-id="c9f05-111">すべて</span><span class="sxs-lookup"><span data-stu-id="c9f05-111">all</span></span>|<span data-ttu-id="c9f05-112">1</span><span class="sxs-lookup"><span data-stu-id="c9f05-112">-1</span></span>|<span data-ttu-id="c9f05-113">半期チャネル (対象指定)</span><span class="sxs-lookup"><span data-stu-id="c9f05-113">Semi-Annual Channel (Targeted)</span></span> <span data-ttu-id="c9f05-114">デバイスでは、半年のチャネル (対象) からすべての適用可能な機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="c9f05-114">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="c9f05-115">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="c9f05-115">businessReadyOnly</span></span>|<span data-ttu-id="c9f05-116">2</span><span class="sxs-lookup"><span data-stu-id="c9f05-116">-2</span></span>|<span data-ttu-id="c9f05-117">半期チャネル</span><span class="sxs-lookup"><span data-stu-id="c9f05-117">Semi-Annual Channel</span></span> <span data-ttu-id="c9f05-118">デバイスは、半年のチャネルからの機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="c9f05-118">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="c9f05-119">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="c9f05-119">windowsInsiderBuildFast</span></span>|<span data-ttu-id="c9f05-120">3</span><span class="sxs-lookup"><span data-stu-id="c9f05-120">"3"</span></span>|<span data-ttu-id="c9f05-121">Windows の内部からのビルド - 高速</span><span class="sxs-lookup"><span data-stu-id="c9f05-121">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="c9f05-122">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="c9f05-122">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="c9f05-123">4</span><span class="sxs-lookup"><span data-stu-id="c9f05-123">-4</span></span>|<span data-ttu-id="c9f05-124">Windows 内部からビルド時間がかかる</span><span class="sxs-lookup"><span data-stu-id="c9f05-124">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="c9f05-125">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="c9f05-125">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="c9f05-126">5</span><span class="sxs-lookup"><span data-stu-id="c9f05-126">.5</span></span>|<span data-ttu-id="c9f05-127">リリース ビルドの Windows の内部から</span><span class="sxs-lookup"><span data-stu-id="c9f05-127">Release Windows Insider build</span></span>|








