---
title: Intune のデバイスとアプリの API の概要
description: 'Microsoft Intune は、企業が組織内のデバイスとアプリを管理するのに役立ちます。 Microsoft Graph で Intune API を使用して、デバイスとアプリを管理したり、好みのツールを使用しながら Intune を構成したりできます。 '
author: tfitzmac
ms.openlocfilehash: 0eac57d7434e85faae86a7f1042cc6bb61783e52
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332852"
---
# <a name="intune-devices-and-apps-api-overview"></a><span data-ttu-id="c15f8-104">Intune のデバイスとアプリの API の概要</span><span class="sxs-lookup"><span data-stu-id="c15f8-104">Intune devices and apps API overview</span></span>

<span data-ttu-id="c15f8-105">Microsoft Intune は、企業が組織内のデバイスとアプリを管理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="c15f8-105">Microsoft Intune helps enterprises manage devices and apps within an organization.</span></span> <span data-ttu-id="c15f8-106">Microsoft Graph で Intune API を使用して、デバイスとアプリを管理したり、好みのツールを使用しながら Intune を構成したりできます。</span><span class="sxs-lookup"><span data-stu-id="c15f8-106">You can use the Intune API in Microsoft Graph to manage devices, apps, and even configure Intune while using your preferred tools.</span></span> 

<span data-ttu-id="c15f8-107">ISV の場合は、Intune API を使用してクライアントのテナントを管理することもできます。</span><span class="sxs-lookup"><span data-stu-id="c15f8-107">If you're an ISV, you can also use the Intune API to manage client tenants.</span></span>

## <a name="why-integrate-with-intune"></a><span data-ttu-id="c15f8-108">Intune と統合する理由</span><span class="sxs-lookup"><span data-stu-id="c15f8-108">Why integrate with Intune?</span></span>

<span data-ttu-id="c15f8-109">Microsoft Graph で Intune API を使用して、Intune のデバイスとアプリに関する情報へのアクセス、デバイスの管理、アプリの管理、および Intune の自動化を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="c15f8-109">You can use the Intune API in Microsoft Graph to access Intune device and application information, manage devices, manage apps, and automate Intune.</span></span>

### <a name="manage-devices"></a><span data-ttu-id="c15f8-110">デバイスを管理する</span><span class="sxs-lookup"><span data-stu-id="c15f8-110">Manage devices</span></span>

<span data-ttu-id="c15f8-111">Intune API を使用して次の作業を実行できます。</span><span class="sxs-lookup"><span data-stu-id="c15f8-111">You can use the Intune API to:</span></span>

- <span data-ttu-id="c15f8-112">パスワードの複雑さと期間、暗号化、脅威保護のレベルなどの[デバイス コンプライアンス](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0) ポリシーを定義し、適用する </span><span class="sxs-lookup"><span data-stu-id="c15f8-112">Define and enforce [device compliance](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0) policies, such as password complexity and duration, encryption, threat protection levels, and so on.</span></span>  <span data-ttu-id="c15f8-113">(サポートされるポリシーは、オペレーティング システムとバージョンによって異なる)</span><span class="sxs-lookup"><span data-stu-id="c15f8-113">(Supported policies vary according to operating system and version).</span></span>
- <span data-ttu-id="c15f8-114">デバイスのプラットフォームが Windows、Android、Mac、iOS のどれであるかに関係なく、[企業データを保護](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0)する</span><span class="sxs-lookup"><span data-stu-id="c15f8-114">[Protect company data](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), regardless of whether the device platform is Windows, Android, Mac, or iOS.</span></span>
- <span data-ttu-id="c15f8-115">オペレーティング システムのプラットフォームとバージョン、ドメインのメンバーシップ、構成設定の管理を含む[デバイス構成](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0)ポリシーを作成し、展開する</span><span class="sxs-lookup"><span data-stu-id="c15f8-115">Create and deploy [device configuration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0) policies, including operating system platform/versioning, domain membership, and configuration setting management.</span></span>
- <span data-ttu-id="c15f8-116">制限付きのダウンロード、ネットワーク アクセサリのアクセス、ファイル転送を含むデバイスの[アクセス制御](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0)ポリシーを作成し、展開する</span><span class="sxs-lookup"><span data-stu-id="c15f8-116">Create and deploy device [access control](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) policies, including restricted download, network accessory access, and file transfer.</span></span>
- <span data-ttu-id="c15f8-117">デバイスの検索、パスワードの変更、デバイスのワイプなどの[リモート アクション](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0)を実行する</span><span class="sxs-lookup"><span data-stu-id="c15f8-117">Perform [remote actions](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), such as locate device, change password, and wipe device.</span></span>

### <a name="manage-apps"></a><span data-ttu-id="c15f8-118">アプリの管理</span><span class="sxs-lookup"><span data-stu-id="c15f8-118">Manage apps</span></span> 

<span data-ttu-id="c15f8-119">Intune API を使用して、次のアプリ管理タスクを実行できます。</span><span class="sxs-lookup"><span data-stu-id="c15f8-119">You can use the Intune API to perform the following app management tasks:</span></span>

- <span data-ttu-id="c15f8-120">[アプリをデバイスに](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0)展開する、またはアプリの展開を禁止する</span><span class="sxs-lookup"><span data-stu-id="c15f8-120">Deploy [apps to devices](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) or prevent apps from being deployed.</span></span>
- <span data-ttu-id="c15f8-121">[電子ブック](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0)と関連サービスへのアクセスを管理する</span><span class="sxs-lookup"><span data-stu-id="c15f8-121">Manage access to [ebooks](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) and related services.</span></span>
- <span data-ttu-id="c15f8-122">アプリ構成設定、アプリ保護設定、およびアプリ使用ポリシーを定義し、展開する</span><span class="sxs-lookup"><span data-stu-id="c15f8-122">Define and deploy app configuration settings, app protection settings, and app usage policies.</span></span>

### <a name="automate-intune"></a><span data-ttu-id="c15f8-123">Intune の自動化</span><span class="sxs-lookup"><span data-stu-id="c15f8-123">Automate Intune</span></span>

<span data-ttu-id="c15f8-124">Intune API を使用して、Intune の次の作業を自動化します。</span><span class="sxs-lookup"><span data-stu-id="c15f8-124">Automate Intune by using the Intune API to:</span></span>

- <span data-ttu-id="c15f8-125">[ロール ベース](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0)のアクセス制御を定義し、割り当てる</span><span class="sxs-lookup"><span data-stu-id="c15f8-125">Define and assign [role based](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0) access controls.</span></span>
- <span data-ttu-id="c15f8-126">コンプライアンス、使用状況、およびアクセスを監査し、レポートする</span><span class="sxs-lookup"><span data-stu-id="c15f8-126">Audit and report compliance, usage, and access.</span></span>
- <span data-ttu-id="c15f8-127">[通信費](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0)を管理する</span><span class="sxs-lookup"><span data-stu-id="c15f8-127">Manage [telecom expenses](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).</span></span>

## <a name="api-reference"></a><span data-ttu-id="c15f8-128">API リファレンス</span><span class="sxs-lookup"><span data-stu-id="c15f8-128">API reference</span></span>
<span data-ttu-id="c15f8-129">このサービスの API リファレンスをお探しですか?</span><span class="sxs-lookup"><span data-stu-id="c15f8-129">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="c15f8-130">Microsoft Graph v1.0 の Intune API</span><span class="sxs-lookup"><span data-stu-id="c15f8-130">Intune API in Microsoft Graph v1.0</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [<span data-ttu-id="c15f8-131">Microsoft Graph ベータ版の Intune API</span><span class="sxs-lookup"><span data-stu-id="c15f8-131">Intune API in Microsoft Graph beta</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="c15f8-132">次のステップ</span><span class="sxs-lookup"><span data-stu-id="c15f8-132">Next steps</span></span>

- <span data-ttu-id="c15f8-133">[Azure AD を使用して Intune API にアクセス](https://docs.microsoft.com/intune/intune-graph-apis)します。</span><span class="sxs-lookup"><span data-stu-id="c15f8-133">[Use Azure AD to access the Intune API](https://docs.microsoft.com/intune/intune-graph-apis).</span></span>
- <span data-ttu-id="c15f8-134">[PowerShell Intune サンプル](https://github.com/microsoftgraph/powershell-intune-samples)を使用して、一般的なタスクの実行方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="c15f8-134">See how to perform common tasks by using the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples).</span></span>
- <span data-ttu-id="c15f8-135">[Intune REST API の使用](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="c15f8-135">Find out how to [use the Intune REST API](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="c15f8-136">[Changelog](changelog.md) で Intune API の最新情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="c15f8-136">See the [Changelog](changelog.md) for information about what's new in the Intune API.</span></span>
- <span data-ttu-id="c15f8-137">Microsoft Graph の使用方法についてのさらに多くのアイデアについては、[サンプル](https://developer.microsoft.com/graph/graph/examples)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c15f8-137">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
