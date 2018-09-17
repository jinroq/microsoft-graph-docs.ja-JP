# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="84f68-101">automaticUpdateMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="84f68-101">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="84f68-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="84f68-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84f68-103">自動更新モードを使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="84f68-103">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="84f68-104">メンバー</span><span class="sxs-lookup"><span data-stu-id="84f68-104">Members</span></span>
|<span data-ttu-id="84f68-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="84f68-105">Member</span></span>|<span data-ttu-id="84f68-106">値</span><span class="sxs-lookup"><span data-stu-id="84f68-106">Value</span></span>|<span data-ttu-id="84f68-107">説明</span><span class="sxs-lookup"><span data-stu-id="84f68-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84f68-108">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="84f68-108">UserDefined</span></span>|<span data-ttu-id="84f68-109">0</span><span class="sxs-lookup"><span data-stu-id="84f68-109">0%</span></span>|<span data-ttu-id="84f68-110">ユーザー定義済み、既定値、目的なし。</span><span class="sxs-lookup"><span data-stu-id="84f68-110">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="84f68-111">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="84f68-111">notifyDownload</span></span>|<span data-ttu-id="84f68-112">1</span><span class="sxs-lookup"><span data-stu-id="84f68-112">-1</span></span>|<span data-ttu-id="84f68-113">ダウンロード時に通知。</span><span class="sxs-lookup"><span data-stu-id="84f68-113">Notify on download.</span></span>|
|<span data-ttu-id="84f68-114">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="84f68-114">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="84f68-115">2</span><span class="sxs-lookup"><span data-stu-id="84f68-115">-2</span></span>|<span data-ttu-id="84f68-116">メンテナンス時に自動インストール。</span><span class="sxs-lookup"><span data-stu-id="84f68-116">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="84f68-117">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="84f68-117">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="84f68-118">3</span><span class="sxs-lookup"><span data-stu-id="84f68-118">"3"</span></span>|<span data-ttu-id="84f68-119">メンテナンス時に自動インストールと再起動。</span><span class="sxs-lookup"><span data-stu-id="84f68-119">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="84f68-120">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="84f68-120">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="84f68-121">4</span><span class="sxs-lookup"><span data-stu-id="84f68-121">-4</span></span>|<span data-ttu-id="84f68-122">設定時刻に自動インストールと再起動。</span><span class="sxs-lookup"><span data-stu-id="84f68-122">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="84f68-123">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="84f68-123">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="84f68-124">5</span><span class="sxs-lookup"><span data-stu-id="84f68-124">.5</span></span>|<span data-ttu-id="84f68-125">エンド ユーザーによる操作なしに自動インストールと再起動。</span><span class="sxs-lookup"><span data-stu-id="84f68-125">Auto-install and restart without end-user control</span></span>|








