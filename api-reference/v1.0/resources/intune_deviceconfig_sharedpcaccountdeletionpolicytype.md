# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="9de11-101">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9de11-101">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="9de11-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9de11-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9de11-103">共有の PC でアカウントが削除されたときに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="9de11-103">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="9de11-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="9de11-104">Members</span></span>
|<span data-ttu-id="9de11-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="9de11-105">Member</span></span>|<span data-ttu-id="9de11-106">値</span><span class="sxs-lookup"><span data-stu-id="9de11-106">Value</span></span>|<span data-ttu-id="9de11-107">説明</span><span class="sxs-lookup"><span data-stu-id="9de11-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9de11-108">イミディ エイト</span><span class="sxs-lookup"><span data-stu-id="9de11-108">immediate</span></span>|<span data-ttu-id="9de11-109">0</span><span class="sxs-lookup"><span data-stu-id="9de11-109">0</span></span>|<span data-ttu-id="9de11-110">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="9de11-110">Delete immediately.</span></span>|
|<span data-ttu-id="9de11-111">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="9de11-111">diskSpaceThreshold</span></span>|<span data-ttu-id="9de11-112">1</span><span class="sxs-lookup"><span data-stu-id="9de11-112">1</span></span>|<span data-ttu-id="9de11-113">ディスク容量のしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="9de11-113">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="9de11-114">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="9de11-114">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="9de11-115">2</span><span class="sxs-lookup"><span data-stu-id="9de11-115">2</span></span>|<span data-ttu-id="9de11-116">ディスク容量のしきい値または非アクティブのしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="9de11-116">Delete at disk space threshold or inactive threshold.</span></span>|



