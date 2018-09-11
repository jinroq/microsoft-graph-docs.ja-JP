# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="c8948-101">defenderThreatAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="c8948-101">defenderThreatAction enum type</span></span>

> <span data-ttu-id="c8948-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8948-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8948-103">マルウェアの脅威を検出するための Defender の既定のアクションです。</span><span class="sxs-lookup"><span data-stu-id="c8948-103">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="c8948-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="c8948-104">Members</span></span>
|<span data-ttu-id="c8948-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="c8948-105">Member</span></span>|<span data-ttu-id="c8948-106">値</span><span class="sxs-lookup"><span data-stu-id="c8948-106">Value</span></span>|<span data-ttu-id="c8948-107">説明</span><span class="sxs-lookup"><span data-stu-id="c8948-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8948-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c8948-108">deviceDefault</span></span>|<span data-ttu-id="c8948-109">0</span><span class="sxs-lookup"><span data-stu-id="c8948-109">0%</span></span>|<span data-ttu-id="c8948-110">更新の定義に基づいてアクションを適用します。</span><span class="sxs-lookup"><span data-stu-id="c8948-110">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="c8948-111">clean</span><span class="sxs-lookup"><span data-stu-id="c8948-111">clean</span></span>|<span data-ttu-id="c8948-112">1</span><span class="sxs-lookup"><span data-stu-id="c8948-112">-1</span></span>|<span data-ttu-id="c8948-113">検出された脅威をクリーンアップします。</span><span class="sxs-lookup"><span data-stu-id="c8948-113">Clean the detected threat.</span></span>|
|<span data-ttu-id="c8948-114">quarantine</span><span class="sxs-lookup"><span data-stu-id="c8948-114">Quarantine</span></span>|<span data-ttu-id="c8948-115">2</span><span class="sxs-lookup"><span data-stu-id="c8948-115">-2</span></span>|<span data-ttu-id="c8948-116">検出された脅威を隔離します。</span><span class="sxs-lookup"><span data-stu-id="c8948-116">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="c8948-117">remove</span><span class="sxs-lookup"><span data-stu-id="c8948-117">remove</span></span>|<span data-ttu-id="c8948-118">3</span><span class="sxs-lookup"><span data-stu-id="c8948-118">"3"</span></span>|<span data-ttu-id="c8948-119">検出された脅威を削除します。</span><span class="sxs-lookup"><span data-stu-id="c8948-119">Remove the detected threat.</span></span>|
|<span data-ttu-id="c8948-120">allow</span><span class="sxs-lookup"><span data-stu-id="c8948-120">Allow</span></span>|<span data-ttu-id="c8948-121">4</span><span class="sxs-lookup"><span data-stu-id="c8948-121">-4</span></span>|<span data-ttu-id="c8948-122">検出された脅威を許可します。</span><span class="sxs-lookup"><span data-stu-id="c8948-122">Allow the detected threat.</span></span>|
|<span data-ttu-id="c8948-123">userDefined</span><span class="sxs-lookup"><span data-stu-id="c8948-123">UserDefined</span></span>|<span data-ttu-id="c8948-124">5</span><span class="sxs-lookup"><span data-stu-id="c8948-124">.5</span></span>|<span data-ttu-id="c8948-125">検出された脅威に対して実行するアクションをユーザーが決定することを許可します。</span><span class="sxs-lookup"><span data-stu-id="c8948-125">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="c8948-126">block</span><span class="sxs-lookup"><span data-stu-id="c8948-126">block</span></span>|<span data-ttu-id="c8948-127">6</span><span class="sxs-lookup"><span data-stu-id="c8948-127">-6</span></span>|<span data-ttu-id="c8948-128">検出された脅威をブロックします。</span><span class="sxs-lookup"><span data-stu-id="c8948-128">Block the detected threat.</span></span>|








