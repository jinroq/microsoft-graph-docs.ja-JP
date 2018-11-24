# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="d1a73-101">vppTokenSyncStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="d1a73-101">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="d1a73-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d1a73-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1a73-103">Apple ボリューム購入プログラム、トークンに関連付けられている可能性のある同期のステータス。</span><span class="sxs-lookup"><span data-stu-id="d1a73-103">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="d1a73-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1a73-104">Members</span></span>
|<span data-ttu-id="d1a73-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1a73-105">Member</span></span>|<span data-ttu-id="d1a73-106">値</span><span class="sxs-lookup"><span data-stu-id="d1a73-106">Value</span></span>|<span data-ttu-id="d1a73-107">説明</span><span class="sxs-lookup"><span data-stu-id="d1a73-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1a73-108">none</span><span class="sxs-lookup"><span data-stu-id="d1a73-108">none</span></span>|<span data-ttu-id="d1a73-109">0</span><span class="sxs-lookup"><span data-stu-id="d1a73-109">0</span></span>|<span data-ttu-id="d1a73-110">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="d1a73-110">Default status.</span></span>|
|<span data-ttu-id="d1a73-111">inProgress</span><span class="sxs-lookup"><span data-stu-id="d1a73-111">inProgress</span></span>|<span data-ttu-id="d1a73-112">1</span><span class="sxs-lookup"><span data-stu-id="d1a73-112">1</span></span>|<span data-ttu-id="d1a73-113">進行中の最後の同期します。</span><span class="sxs-lookup"><span data-stu-id="d1a73-113">Last Sync in progress.</span></span>|
|<span data-ttu-id="d1a73-114">完了</span><span class="sxs-lookup"><span data-stu-id="d1a73-114">completed</span></span>|<span data-ttu-id="d1a73-115">2</span><span class="sxs-lookup"><span data-stu-id="d1a73-115">2</span></span>|<span data-ttu-id="d1a73-116">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="d1a73-116">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="d1a73-117">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="d1a73-117">failed</span></span>|<span data-ttu-id="d1a73-118">3</span><span class="sxs-lookup"><span data-stu-id="d1a73-118">3</span></span>|<span data-ttu-id="d1a73-119">前回の同期が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="d1a73-119">Last Sync failed.</span></span>|



