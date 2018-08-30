# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="29b32-101">sharedPCAccountManagerPolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="29b32-101">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="29b32-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29b32-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29b32-103">共有 PC アカウント マネージャー ポリシーです。</span><span class="sxs-lookup"><span data-stu-id="29b32-103">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="29b32-104">アカウント マネージャーが有効になっている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="29b32-104">Only applies when the account manager is enabled.</span></span>
## <a name="properties"></a><span data-ttu-id="29b32-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29b32-105">Properties</span></span>
|<span data-ttu-id="29b32-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29b32-106">Property</span></span>|<span data-ttu-id="29b32-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="29b32-107">Type</span></span>|<span data-ttu-id="29b32-108">説明</span><span class="sxs-lookup"><span data-stu-id="29b32-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29b32-109">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="29b32-109">accountDeletionPolicy</span></span>|[<span data-ttu-id="29b32-110">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="29b32-110">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune_deviceconfig_sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="29b32-111">アカウントの削除のタイミングを構成します。</span><span class="sxs-lookup"><span data-stu-id="29b32-111">Configures when accounts are deleted.</span></span> <span data-ttu-id="29b32-112">指定できる値は、`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold` です。</span><span class="sxs-lookup"><span data-stu-id="29b32-112">The possible values are `immediate`, `diskSpaceThreshold`, or `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="29b32-113">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="29b32-113">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="29b32-114">Int32</span><span class="sxs-lookup"><span data-stu-id="29b32-114">Int32</span></span>|<span data-ttu-id="29b32-115">キャッシュされている共有 PC アカウントの削除が停止される前に、PC に必要な使用可能なディスク領域の割合を設定します。</span><span class="sxs-lookup"><span data-stu-id="29b32-115">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="29b32-116">AccountDeletionPolicy が DiskSpaceThreshold または DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="29b32-116">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="29b32-117">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="29b32-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="29b32-118">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="29b32-118">inactiveThresholdDays</span></span>|<span data-ttu-id="29b32-119">Int32</span><span class="sxs-lookup"><span data-stu-id="29b32-119">Int32</span></span>|<span data-ttu-id="29b32-120">指定した期間にわたってログオンしていない場合にアカウントの削除が始まるタイミングを日数で指定します。</span><span class="sxs-lookup"><span data-stu-id="29b32-120">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="29b32-121">AccountDeletionPolicy が DiskSpaceThreshold または DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="29b32-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="29b32-122">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="29b32-122">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="29b32-123">Int32</span><span class="sxs-lookup"><span data-stu-id="29b32-123">Int32</span></span>|<span data-ttu-id="29b32-124">キャッシュ済みのアカウントを削除してディスク領域を空ける前に、PC に残っているディスク領域の割合を設定します。</span><span class="sxs-lookup"><span data-stu-id="29b32-124">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="29b32-125">非アクティブの状態が最長のアカウントから削除されます。</span><span class="sxs-lookup"><span data-stu-id="29b32-125">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="29b32-126">AccountDeletionPolicy が DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="29b32-126">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="29b32-127">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="29b32-127">Valid values 0 to 100</span></span>|


## <a name="relationships"></a><span data-ttu-id="29b32-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29b32-128">Relationships</span></span>
<span data-ttu-id="29b32-129">なし</span><span class="sxs-lookup"><span data-stu-id="29b32-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="29b32-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29b32-130">JSON Representation</span></span>
<span data-ttu-id="29b32-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29b32-131">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```



