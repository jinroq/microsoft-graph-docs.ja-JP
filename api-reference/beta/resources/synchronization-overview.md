---
title: Azure AD 同期 API の概要
description: )、作成を自動化することにより、保守、および id の削除クラウド (ソフトウェア、サービス、または saas のどちらとして) アプリケーションをドロップ ボックス、セールス、ServiceNow などです。 使用できます同期 Api Graph でプログラムを使用して、id の同期を管理するのになど。
localization_priority: Normal
ms.openlocfilehash: ed994b8204fdee38f558da499259538e85eacd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529559"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="51e57-104">Azure AD 同期 API の概要</span><span class="sxs-lookup"><span data-stu-id="51e57-104">Azure AD synchronization API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51e57-105">(「プロビジョニング」とも呼ばれます)、azure Active Directory (AD の Azure) id の同期を使用すると、作成、保守、およびクラウド (SaaS サービスとしてのソフトウェア) の id の削除を自動化するアプリケーションをドロップ ボックス セールス ServiceNow、など。</span><span class="sxs-lookup"><span data-stu-id="51e57-105">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="51e57-106">使用できます同期 Api Graph でプログラムを使用して、id の同期を管理するのになど。</span><span class="sxs-lookup"><span data-stu-id="51e57-106">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="51e57-107">作成、起動、および同期ジョブを停止します。</span><span class="sxs-lookup"><span data-stu-id="51e57-107">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="51e57-108">ジョブの同期スキーマに変更を加える</span><span class="sxs-lookup"><span data-stu-id="51e57-108">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="51e57-109">現在の同期状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="51e57-109">Verify the current synchronization status</span></span> 

<span data-ttu-id="51e57-110">Azure AD での同期の詳細についてを参照してください。</span><span class="sxs-lookup"><span data-stu-id="51e57-110">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="51e57-111">ユーザー プロビジョニングと Azure Active Directory を使用して、SaaS アプリケーションをプロビジョニング解除の自動化します。</span><span class="sxs-lookup"><span data-stu-id="51e57-111">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="51e57-112">Azure ポータル エンタープライズ アプリケーションのプロビジョニングのユーザー アカウントを管理します。</span><span class="sxs-lookup"><span data-stu-id="51e57-112">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="51e57-113">サンプルのテナントや、独自のテナントでの[グラフのエクスプ ローラー](https://developer.microsoft.com/graph/graph-explorer)の API を試みることができます。</span><span class="sxs-lookup"><span data-stu-id="51e57-113">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="51e57-114">同期ジョブ</span><span class="sxs-lookup"><span data-stu-id="51e57-114">Synchronization job</span></span>

<span data-ttu-id="51e57-115">同期ジョブは、バック グラウンドで定期的に実行している、1 つのディレクトリと別のディレクトリにプッシュすることで変更をポーリングして同期を実行します。</span><span class="sxs-lookup"><span data-stu-id="51e57-115">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="51e57-116">同期ジョブは、テナントにアプリケーションの特定のインスタンスに固有では常にします。</span><span class="sxs-lookup"><span data-stu-id="51e57-116">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="51e57-117">同期ジョブの設定の一部として、ターゲット ディレクトリにオブジェクトを読み書きするための承認を与えると、ジョブの同期スキーマをカスタマイズする必要があります。</span><span class="sxs-lookup"><span data-stu-id="51e57-117">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="51e57-118">詳細については、[同期ジョブ](synchronization-synchronizationjob.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51e57-118">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="51e57-119">同期スキーマ</span><span class="sxs-lookup"><span data-stu-id="51e57-119">Synchronization schema</span></span>

<span data-ttu-id="51e57-120">同期スキーマで定義されるオブジェクトの同期し、同期する方法です。</span><span class="sxs-lookup"><span data-stu-id="51e57-120">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="51e57-121">同期スキーマには、特定の同期ジョブのセットアップ情報のほとんどが含まれています。</span><span class="sxs-lookup"><span data-stu-id="51e57-121">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="51e57-122">通常、[属性マッピング](synchronization-attributemapping.md)の一部をカスタマイズまたはを特定の条件を満たすオブジェクトのみを同期する[スコープのフィルター](synchronization-filter.md)が追加されます。</span><span class="sxs-lookup"><span data-stu-id="51e57-122">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="51e57-123">同期スキーマには、次のコンポーネントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="51e57-123">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="51e57-124">ディレクトリの定義</span><span class="sxs-lookup"><span data-stu-id="51e57-124">Directory definitions</span></span>
- <span data-ttu-id="51e57-125">同期ルール</span><span class="sxs-lookup"><span data-stu-id="51e57-125">Synchronization rules</span></span>
- <span data-ttu-id="51e57-126">オブジェクトのマッピング</span><span class="sxs-lookup"><span data-stu-id="51e57-126">Object mappings</span></span>

<span data-ttu-id="51e57-127">詳細については、[同期スキーマ](synchronization-synchronizationschema.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51e57-127">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="51e57-128">同期テンプレート</span><span class="sxs-lookup"><span data-stu-id="51e57-128">Synchronization template</span></span>

<span data-ttu-id="51e57-129">同期テンプレートは、特定のアプリケーションの構成済みの同期設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="51e57-129">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="51e57-130">(最も重要なは、[同期スキーマ](synchronization-synchronizationschema.md)) は、これらの設定は、テンプレートに基づくすべての[同期ジョブ](synchronization-synchronizationjob.md)の既定で使用されます。</span><span class="sxs-lookup"><span data-stu-id="51e57-130">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="51e57-131">テンプレートは、アプリケーション開発者によって指定されます。</span><span class="sxs-lookup"><span data-stu-id="51e57-131">Templates are specified by the application developer.</span></span>

<span data-ttu-id="51e57-132">詳細については、[同期のテンプレート](synchronization-synchronizationtemplate.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51e57-132">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="51e57-133">同期 API を使用します。</span><span class="sxs-lookup"><span data-stu-id="51e57-133">Working with the synchronization API</span></span>

<span data-ttu-id="51e57-134">同期を使用する API の主要部分は[synchronizationJob](synchronization-synchronizationjob.md)と[synchronizationSchema](synchronization-synchronizationschema.md)のリソースにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="51e57-134">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="51e57-135">[SynchronizationJob](synchronization-synchronizationjob.md)リソースを検索するには、同期ジョブが属するサービスのプリンシパル オブジェクトの ID を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="51e57-135">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="51e57-136">次の例では、 **synchronizationJob**と**synchronizationSchema**のリソースを操作する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="51e57-136">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="51e57-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="51e57-137">Authorization</span></span>

<span data-ttu-id="51e57-138">Azure AD 同期 API では、OAuth 2.0 を使用して、承認のため。</span><span class="sxs-lookup"><span data-stu-id="51e57-138">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="51e57-139">API へのすべての要求を行う前に、アクセス トークンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="51e57-139">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="51e57-140">詳細については、 [Microsoft Graph を呼び出すための Get アクセス トークン](https://developer.microsoft.com/graph/docs/concepts/auth_overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51e57-140">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="51e57-141">同期リソースにアクセスするには、アプリケーションには、Directory.ReadWrite.All のアクセス許可が必要があります。</span><span class="sxs-lookup"><span data-stu-id="51e57-141">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="51e57-142">詳細については、[ディレクトリのアクセス許可](/graph/permissions-reference#directory-permissions)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51e57-142">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="51e57-143">サービスのプリンシパル オブジェクトを表示名で検索します。</span><span class="sxs-lookup"><span data-stu-id="51e57-143">Find the service principal object by display name</span></span>

<span data-ttu-id="51e57-144">次の例では、表示名でサービスのプリンシパル オブジェクトを検索する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="51e57-144">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="51e57-145">要求</span><span class="sxs-lookup"><span data-stu-id="51e57-145">**Request**</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="51e57-146">**応答**</span><span class="sxs-lookup"><span data-stu-id="51e57-146">**Response**</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="51e57-147">アプリケーション id サービスのプリンシパル オブジェクトを検索します。</span><span class="sxs-lookup"><span data-stu-id="51e57-147">Find the service principal object by app ID</span></span>

<span data-ttu-id="51e57-148">次の使用例は、アプリケーション id サービスのプリンシパル オブジェクトを検索する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="51e57-148">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="51e57-149">要求</span><span class="sxs-lookup"><span data-stu-id="51e57-149">**Request** 
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="51e57-150">応答</span><span class="sxs-lookup"><span data-stu-id="51e57-150">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="51e57-151">既存の同期ジョブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="51e57-151">List existing synchronization jobs</span></span>

<span data-ttu-id="51e57-152">次の使用例は、既存の同期ジョブを一覧表示する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="51e57-152">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="51e57-153">要求</span><span class="sxs-lookup"><span data-stu-id="51e57-153">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="51e57-154">応答</span><span class="sxs-lookup"><span data-stu-id="51e57-154">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a><span data-ttu-id="51e57-155">同期ジョブのステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="51e57-155">Get synchronization job status</span></span>
<span data-ttu-id="51e57-156">次の例では、同期ジョブのステータスを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="51e57-156">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="51e57-157">要求</span><span class="sxs-lookup"><span data-stu-id="51e57-157">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="51e57-158">応答</span><span class="sxs-lookup"><span data-stu-id="51e57-158">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a><span data-ttu-id="51e57-159">同期スキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="51e57-159">Get synchronization schema</span></span>
<span data-ttu-id="51e57-160">次の例では、同期スキーマを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="51e57-160">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="51e57-161">要求</span><span class="sxs-lookup"><span data-stu-id="51e57-161">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="51e57-162">応答</span><span class="sxs-lookup"><span data-stu-id="51e57-162">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="51e57-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="51e57-163">See also</span></span>

* [<span data-ttu-id="51e57-164">ディレクトリの拡張属性を使用して同期を構成します。</span><span class="sxs-lookup"><span data-stu-id="51e57-164">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="51e57-165">カスタム ターゲットの属性を使用して同期を構成します。</span><span class="sxs-lookup"><span data-stu-id="51e57-165">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
