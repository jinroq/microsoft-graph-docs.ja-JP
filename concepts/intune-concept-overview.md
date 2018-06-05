# <a name="intune-devices-and-apps-api-overview"></a><span data-ttu-id="4ded7-101">Intune のデバイスとアプリの API の概要</span><span class="sxs-lookup"><span data-stu-id="4ded7-101">Intune devices and apps API overview</span></span>

<span data-ttu-id="4ded7-102">Microsoft Intune は、企業が組織内のデバイスとアプリを管理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="4ded7-102">Microsoft Intune helps enterprises manage devices and apps within an organization.</span></span> <span data-ttu-id="4ded7-103">Microsoft Graph で Intune API を使用して、デバイスとアプリを管理したり、好みのツールを使用しながら Intune を構成したりできます。</span><span class="sxs-lookup"><span data-stu-id="4ded7-103">You can use the Intune API in Microsoft Graph to manage devices, apps, and even configure Intune while using your preferred tools.</span></span> 

<span data-ttu-id="4ded7-104">ISV の場合は、Intune API を使用してクライアントのテナントを管理することもできます。</span><span class="sxs-lookup"><span data-stu-id="4ded7-104">If you're an ISV, you can also use the Intune API to manage client tenants.</span></span>

## <a name="why-integrate-with-intune"></a><span data-ttu-id="4ded7-105">Intune と統合する理由</span><span class="sxs-lookup"><span data-stu-id="4ded7-105">Why integrate with Intune?</span></span>

<span data-ttu-id="4ded7-106">Microsoft Graph で Intune API を使用して、Intune のデバイスとアプリに関する情報へのアクセス、デバイスの管理、アプリの管理、および Intune の自動化を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="4ded7-106">You can use the Intune API in Microsoft Graph to access Intune device and application information, manage devices, manage apps, and automate Intune.</span></span>

### <a name="manage-devices"></a><span data-ttu-id="4ded7-107">デバイスを管理する</span><span class="sxs-lookup"><span data-stu-id="4ded7-107">Manage devices</span></span>

<span data-ttu-id="4ded7-108">Intune API を使用して次の作業を実行できます。</span><span class="sxs-lookup"><span data-stu-id="4ded7-108">You can use the Intune API to:</span></span>

- <span data-ttu-id="4ded7-109">パスワードの複雑さと期間、暗号化、脅威保護のレベルなどの[デバイス コンプライアンス](../api-reference/v1.0/resources/intune_deviceconfig_devicecomplianceactionitem.md) ポリシーを定義し、適用する </span><span class="sxs-lookup"><span data-stu-id="4ded7-109">Define and enforce [device compliance](../api-reference/v1.0/resources/intune_deviceconfig_devicecomplianceactionitem.md) policies, such as password complexity and duration, encryption, threat protection levels, and so on.</span></span>  <span data-ttu-id="4ded7-110">(サポートされるポリシーは、オペレーティング システムとバージョンによって異なる)</span><span class="sxs-lookup"><span data-stu-id="4ded7-110">(Supported policies vary according to operating system and version).</span></span>
- <span data-ttu-id="4ded7-111">デバイスのプラットフォームが Windows、Android、Mac、iOS のどれであるかに関係なく、[企業データを保護](../api-reference/v1.0/resources/intune_mam_windowsinformationprotectionpolicy.md)する</span><span class="sxs-lookup"><span data-stu-id="4ded7-111">[Protect company data](../api-reference/v1.0/resources/intune_mam_windowsinformationprotectionpolicy.md), regardless of whether the device platform is Windows, Android, Mac, or iOS.</span></span>
- <span data-ttu-id="4ded7-112">オペレーティング システムのプラットフォームとバージョン、ドメインのメンバーシップ、構成設定の管理を含む[デバイス構成](../api-reference/v1.0/resources/intune_deviceconfig_deviceconfiguration.md)ポリシーを作成し、展開する</span><span class="sxs-lookup"><span data-stu-id="4ded7-112">Create and deploy [device configuration](../api-reference/v1.0/resources/intune_deviceconfig_deviceconfiguration.md) policies, including operating system platform/versioning, domain membership, and configuration setting management.</span></span>
- <span data-ttu-id="4ded7-113">制限付きのダウンロード、ネットワーク アクセサリのアクセス、ファイル転送を含むデバイスの[アクセス制御](../api-reference/v1.0/resources/intune_onboarding_onpremisesconditionalaccesssettings.md)ポリシーを作成し、展開する</span><span class="sxs-lookup"><span data-stu-id="4ded7-113">Create and deploy device [access control](../api-reference/v1.0/resources/intune_onboarding_onpremisesconditionalaccesssettings.md) policies, including restricted download, network accessory access, and file transfer.</span></span>
- <span data-ttu-id="4ded7-114">デバイスの検索、パスワードの変更、デバイスのワイプなどの[リモート アクション](../api-reference/v1.0/resources/intune_devices_manageddevice.md)を実行する</span><span class="sxs-lookup"><span data-stu-id="4ded7-114">Perform [remote actions](../api-reference/v1.0/resources/intune_devices_manageddevice.md), such as locate device, change password, and wipe device.</span></span>

### <a name="manage-apps"></a><span data-ttu-id="4ded7-115">アプリの管理</span><span class="sxs-lookup"><span data-stu-id="4ded7-115">Manage apps</span></span> 

<span data-ttu-id="4ded7-116">Intune API を使用して、次のアプリ管理タスクを実行できます。</span><span class="sxs-lookup"><span data-stu-id="4ded7-116">You can use the Intune API to perform the following app management tasks:</span></span>

- <span data-ttu-id="4ded7-117">[アプリをデバイスに](../api-reference/v1.0/resources/intune_apps_mobileapp.md)展開する、またはアプリの展開を禁止する</span><span class="sxs-lookup"><span data-stu-id="4ded7-117">Deploy [apps to devices](../api-reference/v1.0/resources/intune_apps_mobileapp.md) or prevent apps from being deployed.</span></span>
- <span data-ttu-id="4ded7-118">[電子ブック](../api-reference/v1.0/resources/intune_books_ebookinstallsummary.md)と関連サービスへのアクセスを管理する</span><span class="sxs-lookup"><span data-stu-id="4ded7-118">Manage access to [ebooks](../api-reference/v1.0/resources/intune_books_ebookinstallsummary.md) and related services.</span></span>
- <span data-ttu-id="4ded7-119">アプリ構成設定、アプリ保護設定、およびアプリ使用ポリシーを定義し、展開する</span><span class="sxs-lookup"><span data-stu-id="4ded7-119">Define and deploy app configuration settings, app protection settings, and app usage policies.</span></span>

### <a name="automate-intune"></a><span data-ttu-id="4ded7-120">Intune の自動化</span><span class="sxs-lookup"><span data-stu-id="4ded7-120">Automate Intune</span></span>

<span data-ttu-id="4ded7-121">Intune API を使用して、Intune の次の作業を自動化します。</span><span class="sxs-lookup"><span data-stu-id="4ded7-121">Automate Intune by using the Intune API to:</span></span>

- <span data-ttu-id="4ded7-122">[ロール ベース](../api-reference/v1.0/resources/intune_rbac_conceptual.md)のアクセス制御を定義し、割り当てる</span><span class="sxs-lookup"><span data-stu-id="4ded7-122">Define and assign [role based](../api-reference/v1.0/resources/intune_rbac_conceptual.md) access controls.</span></span>
- <span data-ttu-id="4ded7-123">コンプライアンス、使用状況、およびアクセスを監査し、レポートする</span><span class="sxs-lookup"><span data-stu-id="4ded7-123">Audit and report compliance, usage, and access.</span></span>
- <span data-ttu-id="4ded7-124">[通信費](../api-reference/v1.0/resources/intune_tem_conceptual.md)を管理する</span><span class="sxs-lookup"><span data-stu-id="4ded7-124">Manage [telecom expenses](../api-reference/v1.0/resources/intune_tem_conceptual.md).</span></span>


## <a name="next-steps"></a><span data-ttu-id="4ded7-125">次の手順</span><span class="sxs-lookup"><span data-stu-id="4ded7-125">Next steps</span></span>

- <span data-ttu-id="4ded7-126">[Azure AD を使用して Intune API にアクセス](https://docs.microsoft.com/intune/intune-graph-apis)します。</span><span class="sxs-lookup"><span data-stu-id="4ded7-126">[Use Azure AD to access the Intune API](https://docs.microsoft.com/intune/intune-graph-apis).</span></span>
- <span data-ttu-id="4ded7-127">[PowerShell Intune サンプル](https://github.com/microsoftgraph/powershell-intune-samples)を使用して、一般的なタスクの実行方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="4ded7-127">See how to perform common tasks by using the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples).</span></span>
- <span data-ttu-id="4ded7-128">[Intune REST API の使用](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_graph_overview)方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="4ded7-128">Find out how to [use the Intune REST API](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/intune_graph_overview).</span></span>
- <span data-ttu-id="4ded7-129">[Changelog](changelog.md) で Intune API の最新情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="4ded7-129">See the [Changelog](changelog.md) for information about what's new in the Intune API.</span></span>
- <span data-ttu-id="4ded7-130">Microsoft Graph の使用方法についてのさらに多くのアイデアについては、[サンプル](https://developer.microsoft.com/ja-JP/graph/graph/examples)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ded7-130">Explore [examples](https://developer.microsoft.com/ja-JP/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
