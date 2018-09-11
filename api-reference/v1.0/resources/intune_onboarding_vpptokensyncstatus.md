# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="e1e07-101">vppTokenSyncStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="e1e07-101">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="e1e07-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでと同様に顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を所持している必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1e07-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1e07-103">Apple Volume Purchase Program トークンに関連付けられている可能性のある同期の状態。</span><span class="sxs-lookup"><span data-stu-id="e1e07-103">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="e1e07-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="e1e07-104">Members</span></span>
|<span data-ttu-id="e1e07-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="e1e07-105">Member</span></span>|<span data-ttu-id="e1e07-106">値</span><span class="sxs-lookup"><span data-stu-id="e1e07-106">Value</span></span>|<span data-ttu-id="e1e07-107">説明</span><span class="sxs-lookup"><span data-stu-id="e1e07-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1e07-108">なし</span><span class="sxs-lookup"><span data-stu-id="e1e07-108">none</span></span>|<span data-ttu-id="e1e07-109">0</span><span class="sxs-lookup"><span data-stu-id="e1e07-109">0%</span></span>|<span data-ttu-id="e1e07-110">既定の状態。</span><span class="sxs-lookup"><span data-stu-id="e1e07-110">Default status</span></span>|
|<span data-ttu-id="e1e07-111">InProgress</span><span class="sxs-lookup"><span data-stu-id="e1e07-111">InProgress</span></span>|<span data-ttu-id="e1e07-112">1</span><span class="sxs-lookup"><span data-stu-id="e1e07-112">-1</span></span>|<span data-ttu-id="e1e07-113">最新の同期が進行中。</span><span class="sxs-lookup"><span data-stu-id="e1e07-113">Last Sync in progress.</span></span>|
|<span data-ttu-id="e1e07-114">completed</span><span class="sxs-lookup"><span data-stu-id="e1e07-114">Completed?</span></span>|<span data-ttu-id="e1e07-115">2</span><span class="sxs-lookup"><span data-stu-id="e1e07-115">-2</span></span>|<span data-ttu-id="e1e07-116">前回の同期は正常に完了。</span><span class="sxs-lookup"><span data-stu-id="e1e07-116">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="e1e07-117">failed</span><span class="sxs-lookup"><span data-stu-id="e1e07-117">Failed</span></span>|<span data-ttu-id="e1e07-118">3</span><span class="sxs-lookup"><span data-stu-id="e1e07-118">"3"</span></span>|<span data-ttu-id="e1e07-119">前回の同期は失敗。</span><span class="sxs-lookup"><span data-stu-id="e1e07-119">Last Sync failed.</span></span>|








