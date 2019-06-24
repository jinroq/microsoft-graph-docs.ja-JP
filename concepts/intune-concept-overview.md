---
title: Intune のデバイスとアプリの API の概要
description: 'Microsoft Intune は、企業が組織内のデバイスとアプリを管理するのに役立ちます。 Microsoft Graph で Intune API を使用して、デバイスとアプリを管理したり、好みのツールを使用しながら Intune を構成したりできます。 '
author: rolyon
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: a18096f53dfa88bd37b0cad11639c3b2285206e6
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133769"
---
# <a name="intune-devices-and-apps-api-overview"></a><span data-ttu-id="19a8f-104">Intune のデバイスとアプリの API の概要</span><span class="sxs-lookup"><span data-stu-id="19a8f-104">Intune devices and apps API overview</span></span>

<span data-ttu-id="19a8f-105">Microsoft Intune は、企業が組織内のデバイスとアプリを管理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="19a8f-105">Microsoft Intune helps enterprises manage devices and apps within an organization.</span></span> <span data-ttu-id="19a8f-106">Microsoft Graph で Intune API を使用して、デバイスとアプリを管理したり、好みのツールを使用しながら Intune を構成したりできます。</span><span class="sxs-lookup"><span data-stu-id="19a8f-106">You can use the Intune API in Microsoft Graph to manage devices, apps, and even configure Intune while using your preferred tools.</span></span> 

<span data-ttu-id="19a8f-107">ISV の場合は、Intune API を使用してクライアントのテナントを管理することもできます。</span><span class="sxs-lookup"><span data-stu-id="19a8f-107">If you're an ISV, you can also use the Intune API to manage client tenants.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/yU1HeqNmN7A]

## <a name="why-integrate-with-intune"></a><span data-ttu-id="19a8f-108">Intune と統合する理由</span><span class="sxs-lookup"><span data-stu-id="19a8f-108">Why integrate with Intune?</span></span>

<span data-ttu-id="19a8f-109">Microsoft Graph で Intune API を使用して、Intune のデバイスとアプリに関する情報へのアクセス、デバイスの管理、アプリの管理、および Intune の自動化を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="19a8f-109">You can use the Intune API in Microsoft Graph to access Intune device and application information, manage devices, manage apps, and automate Intune.</span></span>

### <a name="manage-devices"></a><span data-ttu-id="19a8f-110">デバイスを管理する</span><span class="sxs-lookup"><span data-stu-id="19a8f-110">Manage devices</span></span>

<span data-ttu-id="19a8f-111">Intune API を使用して次の作業を実行できます。</span><span class="sxs-lookup"><span data-stu-id="19a8f-111">You can use the Intune API to:</span></span>

- <span data-ttu-id="19a8f-112">パスワードの複雑さと期間、暗号化、脅威保護のレベルなどの[デバイス コンプライアンス](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0) ポリシーを定義し、適用する </span><span class="sxs-lookup"><span data-stu-id="19a8f-112">Define and enforce [device compliance](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0) policies, such as password complexity and duration, encryption, threat protection levels, and so on.</span></span>  <span data-ttu-id="19a8f-113">(サポートされるポリシーは、オペレーティング システムとバージョンによって異なる)</span><span class="sxs-lookup"><span data-stu-id="19a8f-113">(Supported policies vary according to operating system and version).</span></span>
- <span data-ttu-id="19a8f-114">デバイスのプラットフォームが Windows、Android、Mac、iOS のどれであるかに関係なく、[企業データを保護](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0)する</span><span class="sxs-lookup"><span data-stu-id="19a8f-114">[Protect company data](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), regardless of whether the device platform is Windows, Android, Mac, or iOS.</span></span>
- <span data-ttu-id="19a8f-115">オペレーティング システムのプラットフォームとバージョン、ドメインのメンバーシップ、構成設定の管理を含む[デバイス構成](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0)ポリシーを作成し、展開する</span><span class="sxs-lookup"><span data-stu-id="19a8f-115">Create and deploy [device configuration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0) policies, including operating system platform/versioning, domain membership, and configuration setting management.</span></span>
- <span data-ttu-id="19a8f-116">制限付きのダウンロード、ネットワーク アクセサリのアクセス、ファイル転送を含むデバイスの[アクセス制御](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0)ポリシーを作成し、展開する</span><span class="sxs-lookup"><span data-stu-id="19a8f-116">Create and deploy device [access control](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) policies, including restricted download, network accessory access, and file transfer.</span></span>
- <span data-ttu-id="19a8f-117">デバイスの検索、パスワードの変更、デバイスのワイプなどの[リモート アクション](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0)を実行する</span><span class="sxs-lookup"><span data-stu-id="19a8f-117">Perform [remote actions](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), such as locate device, change password, and wipe device.</span></span>

### <a name="manage-apps"></a><span data-ttu-id="19a8f-118">アプリの管理</span><span class="sxs-lookup"><span data-stu-id="19a8f-118">Manage apps</span></span> 

<span data-ttu-id="19a8f-119">Intune API を使用して、次のアプリ管理タスクを実行できます。</span><span class="sxs-lookup"><span data-stu-id="19a8f-119">You can use the Intune API to perform the following app management tasks:</span></span>

- <span data-ttu-id="19a8f-120">[アプリをデバイスに](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0)展開する、またはアプリの展開を禁止する</span><span class="sxs-lookup"><span data-stu-id="19a8f-120">Deploy [apps to devices](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) or prevent apps from being deployed.</span></span>
- <span data-ttu-id="19a8f-121">[電子ブック](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0)と関連サービスへのアクセスを管理する</span><span class="sxs-lookup"><span data-stu-id="19a8f-121">Manage access to [ebooks](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) and related services.</span></span>
- <span data-ttu-id="19a8f-122">アプリ構成設定、アプリ保護設定、およびアプリ使用ポリシーを定義し、展開する</span><span class="sxs-lookup"><span data-stu-id="19a8f-122">Define and deploy app configuration settings, app protection settings, and app usage policies.</span></span>

### <a name="automate-intune"></a><span data-ttu-id="19a8f-123">Intune の自動化</span><span class="sxs-lookup"><span data-stu-id="19a8f-123">Automate Intune</span></span>

<span data-ttu-id="19a8f-124">Intune API を使用して、Intune の次の作業を自動化します。</span><span class="sxs-lookup"><span data-stu-id="19a8f-124">Automate Intune by using the Intune API to:</span></span>

- <span data-ttu-id="19a8f-125">[ロール ベース](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0)のアクセス制御を定義し、割り当てる</span><span class="sxs-lookup"><span data-stu-id="19a8f-125">Define and assign [role based](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0) access controls.</span></span>
- <span data-ttu-id="19a8f-126">コンプライアンス、使用状況、およびアクセスを監査し、レポートする</span><span class="sxs-lookup"><span data-stu-id="19a8f-126">Audit and report compliance, usage, and access.</span></span>
- <span data-ttu-id="19a8f-127">[通信費](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0)を管理する</span><span class="sxs-lookup"><span data-stu-id="19a8f-127">Manage [telecom expenses](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).</span></span>

## <a name="api-reference"></a><span data-ttu-id="19a8f-128">API リファレンス</span><span class="sxs-lookup"><span data-stu-id="19a8f-128">API reference</span></span>
<span data-ttu-id="19a8f-129">このサービスの API リファレンスをお探しですか?</span><span class="sxs-lookup"><span data-stu-id="19a8f-129">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="19a8f-130">Microsoft Graph v1.0 の Intune API</span><span class="sxs-lookup"><span data-stu-id="19a8f-130">Intune API in Microsoft Graph v1.0</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [<span data-ttu-id="19a8f-131">Microsoft Graph ベータ版の Intune API</span><span class="sxs-lookup"><span data-stu-id="19a8f-131">Intune API in Microsoft Graph beta</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="19a8f-132">次のステップ</span><span class="sxs-lookup"><span data-stu-id="19a8f-132">Next steps</span></span>

- <span data-ttu-id="19a8f-133">[Azure AD を使用して Intune API にアクセス](https://docs.microsoft.com/intune/intune-graph-apis)します。</span><span class="sxs-lookup"><span data-stu-id="19a8f-133">[Use Azure AD to access the Intune API](https://docs.microsoft.com/intune/intune-graph-apis).</span></span>
- <span data-ttu-id="19a8f-134">[PowerShell Intune サンプル](https://github.com/microsoftgraph/powershell-intune-samples)を使用して、一般的なタスクの実行方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="19a8f-134">See how to perform common tasks by using the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples).</span></span>
- <span data-ttu-id="19a8f-135">[Intune REST API の使用](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="19a8f-135">Find out how to [use the Intune REST API](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="19a8f-136">[Changelog](changelog.md) で Intune API の最新情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="19a8f-136">See the [Changelog](changelog.md) for information about what's new in the Intune API.</span></span>
- <span data-ttu-id="19a8f-137">Microsoft Graph の使用方法についてのさらに多くのアイデアについては、[サンプル](https://developer.microsoft.com/graph/graph/examples)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19a8f-137">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
