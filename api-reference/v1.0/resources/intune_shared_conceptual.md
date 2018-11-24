# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="85531-101">Microsoft Intune 内の共有リソース</span><span class="sxs-lookup"><span data-stu-id="85531-101">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="85531-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="85531-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="85531-103">これらのエンドポイントは、Intune ワークフローの複数の Microsoft グラフ API で使用されます。</span><span class="sxs-lookup"><span data-stu-id="85531-103">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="85531-104">意図、目的、および特定のリソースを使用する必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="85531-104">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="85531-105">さらに、特定のメソッド、プロパティ、およびアクションが特定のワークフローに対してのみサポートします。</span><span class="sxs-lookup"><span data-stu-id="85531-105">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="85531-106">Intune ワークフローとの間は、次のグラフのリソースを共有します。</span><span class="sxs-lookup"><span data-stu-id="85531-106">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="85531-107">すべてのデバイスの割り当て先</span><span class="sxs-lookup"><span data-stu-id="85531-107">All devices assignment target</span></span>](intune_shared_alldevicesassignmenttarget.md)
- [<span data-ttu-id="85531-108">すべてのライセンス ユーザーの割り当て先</span><span class="sxs-lookup"><span data-stu-id="85531-108">All licensed users assignment target</span></span>](intune_shared_alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="85531-109">準拠の状態</span><span class="sxs-lookup"><span data-stu-id="85531-109">Compliance status</span></span>](intune_shared_compliancestatus.md)
- [<span data-ttu-id="85531-110">デバイスおよびアプリ管理の割り当て先</span><span class="sxs-lookup"><span data-stu-id="85531-110">Device and app management assignment target</span></span>](intune_shared_deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="85531-111">デバイス アプリの管理</span><span class="sxs-lookup"><span data-stu-id="85531-111">Device app management</span></span>](intune_shared_deviceappmanagement.md)
- [<span data-ttu-id="85531-112">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="85531-112">Device category</span></span>](intune_shared_devicecategory.md)
- [<span data-ttu-id="85531-113">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="85531-113">Device management</span></span>](intune_shared_devicemanagement.md)
- [<span data-ttu-id="85531-114">除外グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="85531-114">Exclusion group assignment target</span></span>](intune_shared_exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="85531-115">グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="85531-115">Group assignment target</span></span>](intune_shared_groupassignmenttarget.md)
- [<span data-ttu-id="85531-116">目的をインストールします。</span><span class="sxs-lookup"><span data-stu-id="85531-116">Install intent</span></span>](intune_shared_installintent.md)
- [<span data-ttu-id="85531-117">MIME コンテンツ</span><span class="sxs-lookup"><span data-stu-id="85531-117">MIME content</span></span>](intune_shared_mimecontent.md)
- [<span data-ttu-id="85531-118">Report</span><span class="sxs-lookup"><span data-stu-id="85531-118">Report</span></span>](intune_shared_report.md)
- [<span data-ttu-id="85531-119">レポートのルート</span><span class="sxs-lookup"><span data-stu-id="85531-119">Report root</span></span>](intune_shared_reportroot.md)
- [<span data-ttu-id="85531-120">UI 状態の生成オプションを保存</span><span class="sxs-lookup"><span data-stu-id="85531-120">Saved UI state generation options</span></span>](intune_shared_saveduistategenerationoptions.md)
- [<span data-ttu-id="85531-121">URI</span><span class="sxs-lookup"><span data-stu-id="85531-121">URI</span></span>](intune_shared_uri.md)
- [<span data-ttu-id="85531-122">User</span><span class="sxs-lookup"><span data-stu-id="85531-122">User</span></span>](intune_shared_user.md)
- [<span data-ttu-id="85531-123">VPP トークン アカウントの種類</span><span class="sxs-lookup"><span data-stu-id="85531-123">VPP token account type</span></span>](intune_shared_vpptokenaccounttype.md)
