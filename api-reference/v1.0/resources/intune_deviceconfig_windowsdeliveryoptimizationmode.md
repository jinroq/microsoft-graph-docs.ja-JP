# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="0b1dd-101">windowsDeliveryOptimizationMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="0b1dd-101">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="0b1dd-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0b1dd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b1dd-103">ピア配布の配信最適化モード</span><span class="sxs-lookup"><span data-stu-id="0b1dd-103">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="0b1dd-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b1dd-104">Members</span></span>
|<span data-ttu-id="0b1dd-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b1dd-105">Member</span></span>|<span data-ttu-id="0b1dd-106">値</span><span class="sxs-lookup"><span data-stu-id="0b1dd-106">Value</span></span>|<span data-ttu-id="0b1dd-107">説明</span><span class="sxs-lookup"><span data-stu-id="0b1dd-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b1dd-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="0b1dd-108">UserDefined</span></span>|<span data-ttu-id="0b1dd-109">0</span><span class="sxs-lookup"><span data-stu-id="0b1dd-109">0%</span></span>|<span data-ttu-id="0b1dd-110">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="0b1dd-110">Allow the user to set.</span></span>|
|<span data-ttu-id="0b1dd-111">httpOnly</span><span class="sxs-lookup"><span data-stu-id="0b1dd-111">httpOnly</span></span>|<span data-ttu-id="0b1dd-112">1</span><span class="sxs-lookup"><span data-stu-id="0b1dd-112">-1</span></span>|<span data-ttu-id="0b1dd-113">HTTPのみ、ピアリングなし</span><span class="sxs-lookup"><span data-stu-id="0b1dd-113">HTTP only, no peering</span></span>|
|<span data-ttu-id="0b1dd-114">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="0b1dd-114">httpWithPeeringNat</span></span>|<span data-ttu-id="0b1dd-115">2</span><span class="sxs-lookup"><span data-stu-id="0b1dd-115">-2</span></span>|<span data-ttu-id="0b1dd-116">OS の既定値 – 同じネットワーク アドレス変換器の背後にあるピアリングとブレンドされた http</span><span class="sxs-lookup"><span data-stu-id="0b1dd-116">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="0b1dd-117">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="0b1dd-117">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="0b1dd-118">3</span><span class="sxs-lookup"><span data-stu-id="0b1dd-118">"3"</span></span>|<span data-ttu-id="0b1dd-119">プライベート グループ全体でピアリングとブレンドされた http</span><span class="sxs-lookup"><span data-stu-id="0b1dd-119">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="0b1dd-120">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="0b1dd-120">httpWithInternetPeering</span></span>|<span data-ttu-id="0b1dd-121">4</span><span class="sxs-lookup"><span data-stu-id="0b1dd-121">-4</span></span>|<span data-ttu-id="0b1dd-122">インターネットのピアリングとブレンドされた http</span><span class="sxs-lookup"><span data-stu-id="0b1dd-122">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="0b1dd-123">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="0b1dd-123">simpleDownload</span></span>|<span data-ttu-id="0b1dd-124">99</span><span class="sxs-lookup"><span data-stu-id="0b1dd-124">-99</span></span>|<span data-ttu-id="0b1dd-125">ピアリングのない単純なダウンロード モード</span><span class="sxs-lookup"><span data-stu-id="0b1dd-125">Simple download mode with no peering</span></span>|
|<span data-ttu-id="0b1dd-126">bypassMode</span><span class="sxs-lookup"><span data-stu-id="0b1dd-126">bypassMode</span></span>|<span data-ttu-id="0b1dd-127">100</span><span class="sxs-lookup"><span data-stu-id="0b1dd-127">100%</span></span>|<span data-ttu-id="0b1dd-128">バイパス モードにします。</span><span class="sxs-lookup"><span data-stu-id="0b1dd-128">Bypass mode.</span></span> <span data-ttu-id="0b1dd-129">配信の最適化を使用せず、代わりに BITS を使用</span><span class="sxs-lookup"><span data-stu-id="0b1dd-129">Do not use Delivery Optimization and use BITS instead</span></span>|








