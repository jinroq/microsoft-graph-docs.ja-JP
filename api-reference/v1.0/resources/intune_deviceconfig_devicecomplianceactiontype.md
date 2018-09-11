# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="3accd-101">deviceComplianceActionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="3accd-101">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="3accd-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3accd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3accd-103">スケジュールされたアクションタイプ列挙型</span><span class="sxs-lookup"><span data-stu-id="3accd-103">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="3accd-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="3accd-104">Members</span></span>
|<span data-ttu-id="3accd-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="3accd-105">Member</span></span>|<span data-ttu-id="3accd-106">値</span><span class="sxs-lookup"><span data-stu-id="3accd-106">Value</span></span>|<span data-ttu-id="3accd-107">説明</span><span class="sxs-lookup"><span data-stu-id="3accd-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3accd-108">noAction</span><span class="sxs-lookup"><span data-stu-id="3accd-108">noAction</span></span>|<span data-ttu-id="3accd-109">0</span><span class="sxs-lookup"><span data-stu-id="3accd-109">0%</span></span>|<span data-ttu-id="3accd-110">アクションなし</span><span class="sxs-lookup"><span data-stu-id="3accd-110">No Action</span></span>|
|<span data-ttu-id="3accd-111">通知</span><span class="sxs-lookup"><span data-stu-id="3accd-111">notification</span></span>|<span data-ttu-id="3accd-112">1</span><span class="sxs-lookup"><span data-stu-id="3accd-112">-1</span></span>|<span data-ttu-id="3accd-113">通知を送信</span><span class="sxs-lookup"><span data-stu-id="3accd-113">Send Notification</span></span>|
|<span data-ttu-id="3accd-114">禁止</span><span class="sxs-lookup"><span data-stu-id="3accd-114">block</span></span>|<span data-ttu-id="3accd-115">2</span><span class="sxs-lookup"><span data-stu-id="3accd-115">-2</span></span>|<span data-ttu-id="3accd-116">AAD でデバイスをブロック</span><span class="sxs-lookup"><span data-stu-id="3accd-116">Block the device in AAD</span></span>|
|<span data-ttu-id="3accd-117">インベントリから削除する</span><span class="sxs-lookup"><span data-stu-id="3accd-117">retire action</span></span>|<span data-ttu-id="3accd-118">3</span><span class="sxs-lookup"><span data-stu-id="3accd-118">"3"</span></span>|<span data-ttu-id="3accd-119">デバイスを破棄</span><span class="sxs-lookup"><span data-stu-id="3accd-119">Retire the device</span></span>|
|<span data-ttu-id="3accd-120">ワイプ</span><span class="sxs-lookup"><span data-stu-id="3accd-120">Wipe</span></span>|<span data-ttu-id="3accd-121">4</span><span class="sxs-lookup"><span data-stu-id="3accd-121">-4</span></span>|<span data-ttu-id="3accd-122">デバイスをワイプ</span><span class="sxs-lookup"><span data-stu-id="3accd-122">Wipe the device</span></span>|
|<span data-ttu-id="3accd-123">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="3accd-123">removeResourceAccessProfiles</span></span>|<span data-ttu-id="3accd-124">5</span><span class="sxs-lookup"><span data-stu-id="3accd-124">.5</span></span>|<span data-ttu-id="3accd-125">デバイスからリソースアクセスプロファイルを削除</span><span class="sxs-lookup"><span data-stu-id="3accd-125">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="3accd-126">pushNotification</span><span class="sxs-lookup"><span data-stu-id="3accd-126">pushNotification</span></span>|<span data-ttu-id="3accd-127">9</span><span class="sxs-lookup"><span data-stu-id="3accd-127">-9</span></span>|<span data-ttu-id="3accd-128">デバイスにプッシュ通知を送信します</span><span class="sxs-lookup"><span data-stu-id="3accd-128">Send push notification to device</span></span>|








