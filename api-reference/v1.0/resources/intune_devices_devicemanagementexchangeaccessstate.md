# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="2a97c-101">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="2a97c-101">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="2a97c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a97c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a97c-103">デバイスExchange のアクセスの状態</span><span class="sxs-lookup"><span data-stu-id="2a97c-103">Device Exchange Access State summary</span></span>
## <a name="members"></a><span data-ttu-id="2a97c-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="2a97c-104">Members</span></span>
|<span data-ttu-id="2a97c-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="2a97c-105">Member</span></span>|<span data-ttu-id="2a97c-106">値</span><span class="sxs-lookup"><span data-stu-id="2a97c-106">Value</span></span>|<span data-ttu-id="2a97c-107">説明</span><span class="sxs-lookup"><span data-stu-id="2a97c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a97c-108">なし</span><span class="sxs-lookup"><span data-stu-id="2a97c-108">none</span></span>|<span data-ttu-id="2a97c-109">0</span><span class="sxs-lookup"><span data-stu-id="2a97c-109">0%</span></span>|<span data-ttu-id="2a97c-110">Exchange からはアクセスの状態が検出されませんでした。</span><span class="sxs-lookup"><span data-stu-id="2a97c-110">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="2a97c-111">不明</span><span class="sxs-lookup"><span data-stu-id="2a97c-111">unknown</span></span>|<span data-ttu-id="2a97c-112">1</span><span class="sxs-lookup"><span data-stu-id="2a97c-112">-1</span></span>|<span data-ttu-id="2a97c-113">Exchange へのデバイスのアクセス状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="2a97c-113">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="2a97c-114">許可されています</span><span class="sxs-lookup"><span data-stu-id="2a97c-114">Allowed</span></span>|<span data-ttu-id="2a97c-115">2</span><span class="sxs-lookup"><span data-stu-id="2a97c-115">-2</span></span>|<span data-ttu-id="2a97c-116">デバイスが Exchange へのアクセス権を持っています
</span><span class="sxs-lookup"><span data-stu-id="2a97c-116">Device has access to Exchange</span></span>|
|<span data-ttu-id="2a97c-117">ブロックされています</span><span class="sxs-lookup"><span data-stu-id="2a97c-117">blocked</span></span>|<span data-ttu-id="2a97c-118">3</span><span class="sxs-lookup"><span data-stu-id="2a97c-118">"3"</span></span>|<span data-ttu-id="2a97c-119">デバイスが Exchange内でブロックされています。</span><span class="sxs-lookup"><span data-stu-id="2a97c-119">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="2a97c-120">隔離されています</span><span class="sxs-lookup"><span data-stu-id="2a97c-120">quarantined</span></span>|<span data-ttu-id="2a97c-121">4</span><span class="sxs-lookup"><span data-stu-id="2a97c-121">-4</span></span>|<span data-ttu-id="2a97c-122">デバイスが Exchangeで隔離されています
</span><span class="sxs-lookup"><span data-stu-id="2a97c-122">Device is Quarantined in Exchange</span></span>|



