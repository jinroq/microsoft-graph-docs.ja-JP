# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="cd84e-101">deviceRegistrationState 列挙型</span><span class="sxs-lookup"><span data-stu-id="cd84e-101">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="cd84e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd84e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd84e-103">デバイス登録のステータス。</span><span class="sxs-lookup"><span data-stu-id="cd84e-103">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="cd84e-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="cd84e-104">Members</span></span>
|<span data-ttu-id="cd84e-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="cd84e-105">Member</span></span>|<span data-ttu-id="cd84e-106">値</span><span class="sxs-lookup"><span data-stu-id="cd84e-106">Value</span></span>|<span data-ttu-id="cd84e-107">説明</span><span class="sxs-lookup"><span data-stu-id="cd84e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd84e-108">notRegistered</span><span class="sxs-lookup"><span data-stu-id="cd84e-108">notRegistered</span></span>|<span data-ttu-id="cd84e-109">0</span><span class="sxs-lookup"><span data-stu-id="cd84e-109">0%</span></span>|<span data-ttu-id="cd84e-110">デバイスは登録されていません。</span><span class="sxs-lookup"><span data-stu-id="cd84e-110">The device is not registered.</span></span>|
|<span data-ttu-id="cd84e-111">登録済み</span><span class="sxs-lookup"><span data-stu-id="cd84e-111">Registered</span></span>|<span data-ttu-id="cd84e-112">2</span><span class="sxs-lookup"><span data-stu-id="cd84e-112">-2</span></span>|<span data-ttu-id="cd84e-113">デバイスが登録されています。</span><span class="sxs-lookup"><span data-stu-id="cd84e-113">The device is registered.</span></span>|
|<span data-ttu-id="cd84e-114">破棄</span><span class="sxs-lookup"><span data-stu-id="cd84e-114">Revoked</span></span>|<span data-ttu-id="cd84e-115">3</span><span class="sxs-lookup"><span data-stu-id="cd84e-115">"3"</span></span>|<span data-ttu-id="cd84e-116">デバイスがブロックされている、消去されている、または廃止されています。</span><span class="sxs-lookup"><span data-stu-id="cd84e-116">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="cd84e-117">keyConflict</span><span class="sxs-lookup"><span data-stu-id="cd84e-117">keyConflict</span></span>|<span data-ttu-id="cd84e-118">4</span><span class="sxs-lookup"><span data-stu-id="cd84e-118">-4</span></span>|<span data-ttu-id="cd84e-119">デバイスに重大な競合があります。</span><span class="sxs-lookup"><span data-stu-id="cd84e-119">The device has a key conflict.</span></span>|
|<span data-ttu-id="cd84e-120">approvalPending</span><span class="sxs-lookup"><span data-stu-id="cd84e-120">approvalPending</span></span>|<span data-ttu-id="cd84e-121">5</span><span class="sxs-lookup"><span data-stu-id="cd84e-121">.5</span></span>|<span data-ttu-id="cd84e-122">デバイスは、承認が保留中です。</span><span class="sxs-lookup"><span data-stu-id="cd84e-122">The current SPListItem is pending approval.</span></span>|
|<span data-ttu-id="cd84e-123">certificateReset</span><span class="sxs-lookup"><span data-stu-id="cd84e-123">certificateReset</span></span>|<span data-ttu-id="cd84e-124">6</span><span class="sxs-lookup"><span data-stu-id="cd84e-124">-6</span></span>|<span data-ttu-id="cd84e-125">デバイスの証明書がリセットされました。</span><span class="sxs-lookup"><span data-stu-id="cd84e-125">The device certificate has been reset.</span></span>|
|<span data-ttu-id="cd84e-126">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="cd84e-126">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="cd84e-127">7</span><span class="sxs-lookup"><span data-stu-id="cd84e-127">-7</span></span>|<span data-ttu-id="cd84e-128">デバイスが登録されていません。登録は保留中です。</span><span class="sxs-lookup"><span data-stu-id="cd84e-128">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="cd84e-129">不明</span><span class="sxs-lookup"><span data-stu-id="cd84e-129">unknown</span></span>|<span data-ttu-id="cd84e-130">8</span><span class="sxs-lookup"><span data-stu-id="cd84e-130">-8</span></span>|<span data-ttu-id="cd84e-131">デバイス ライセンス登録のステータスは不明です。</span><span class="sxs-lookup"><span data-stu-id="cd84e-131">The device registration status is unknown.</span></span>|








