# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="b80f7-101">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="b80f7-101">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="b80f7-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b80f7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b80f7-103">デバイスExchange のアクセスの状態</span><span class="sxs-lookup"><span data-stu-id="b80f7-103">Device Exchange Access State summary</span></span>
## <a name="members"></a><span data-ttu-id="b80f7-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="b80f7-104">Members</span></span>
|<span data-ttu-id="b80f7-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="b80f7-105">Member</span></span>|<span data-ttu-id="b80f7-106">値</span><span class="sxs-lookup"><span data-stu-id="b80f7-106">Value</span></span>|<span data-ttu-id="b80f7-107">説明</span><span class="sxs-lookup"><span data-stu-id="b80f7-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b80f7-108">なし</span><span class="sxs-lookup"><span data-stu-id="b80f7-108">none</span></span>|<span data-ttu-id="b80f7-109">0</span><span class="sxs-lookup"><span data-stu-id="b80f7-109">0%</span></span>|<span data-ttu-id="b80f7-110">Exchange からはアクセスの状態が検出されませんでした。</span><span class="sxs-lookup"><span data-stu-id="b80f7-110">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="b80f7-111">不明</span><span class="sxs-lookup"><span data-stu-id="b80f7-111">unknown</span></span>|<span data-ttu-id="b80f7-112">1</span><span class="sxs-lookup"><span data-stu-id="b80f7-112">-1</span></span>|<span data-ttu-id="b80f7-113">Exchange へのデバイスのアクセス状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="b80f7-113">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="b80f7-114">許可されています</span><span class="sxs-lookup"><span data-stu-id="b80f7-114">Allowed</span></span>|<span data-ttu-id="b80f7-115">2</span><span class="sxs-lookup"><span data-stu-id="b80f7-115">-2</span></span>|<span data-ttu-id="b80f7-116">デバイスが Exchange へのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="b80f7-116">Device has access to Exchange</span></span>|
|<span data-ttu-id="b80f7-117">ブロック</span><span class="sxs-lookup"><span data-stu-id="b80f7-117">blocked</span></span>|<span data-ttu-id="b80f7-118">3</span><span class="sxs-lookup"><span data-stu-id="b80f7-118">"3"</span></span>|<span data-ttu-id="b80f7-119">デバイスが Exchange内でブロックされています。</span><span class="sxs-lookup"><span data-stu-id="b80f7-119">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="b80f7-120">隔離されています</span><span class="sxs-lookup"><span data-stu-id="b80f7-120">quarantined</span></span>|<span data-ttu-id="b80f7-121">4</span><span class="sxs-lookup"><span data-stu-id="b80f7-121">-4</span></span>|<span data-ttu-id="b80f7-122">デバイスが Exchangeで隔離されています</span><span class="sxs-lookup"><span data-stu-id="b80f7-122">Device is Quarantined in Exchange</span></span>|








