---
title: Azure AD 同期 API の概要
description: )、作成を自動化することにより、保守、および id の削除クラウド (ソフトウェア、サービス、または saas のどちらとして) アプリケーションをドロップ ボックス、セールス、ServiceNow などです。 使用できます同期 Api Graph でプログラムを使用して、id の同期を管理するのになど。
localization_priority: Normal
ms.openlocfilehash: aada94f39c67fb1174924d49c6e57650f4961cc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884687"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="ddb09-104">Azure AD 同期 API の概要</span><span class="sxs-lookup"><span data-stu-id="ddb09-104">Azure AD synchronization API overview</span></span>

> <span data-ttu-id="ddb09-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ddb09-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddb09-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddb09-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ddb09-107">(「プロビジョニング」とも呼ばれます)、azure Active Directory (AD の Azure) id の同期を使用すると、作成、保守、およびクラウド (SaaS サービスとしてのソフトウェア) の id の削除を自動化するアプリケーションをドロップ ボックス セールス ServiceNow、など。</span><span class="sxs-lookup"><span data-stu-id="ddb09-107">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="ddb09-108">使用できます同期 Api Graph でプログラムを使用して、id の同期を管理するのになど。</span><span class="sxs-lookup"><span data-stu-id="ddb09-108">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="ddb09-109">作成、起動、および同期ジョブを停止します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-109">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="ddb09-110">ジョブの同期スキーマに変更を加える</span><span class="sxs-lookup"><span data-stu-id="ddb09-110">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="ddb09-111">現在の同期状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-111">Verify the current synchronization status</span></span> 

<span data-ttu-id="ddb09-112">Azure AD での同期の詳細についてを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddb09-112">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="ddb09-113">ユーザー プロビジョニングと Azure Active Directory を使用して、SaaS アプリケーションをプロビジョニング解除の自動化します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-113">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="ddb09-114">Azure ポータル エンタープライズ アプリケーションのプロビジョニングのユーザー アカウントを管理します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-114">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="ddb09-115">サンプルのテナントや、独自のテナントでの[グラフのエクスプ ローラー](https://developer.microsoft.com/graph/graph-explorer)の API を試みることができます。</span><span class="sxs-lookup"><span data-stu-id="ddb09-115">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="ddb09-116">同期ジョブ</span><span class="sxs-lookup"><span data-stu-id="ddb09-116">Synchronization job</span></span>

<span data-ttu-id="ddb09-117">同期ジョブは、バック グラウンドで定期的に実行している、1 つのディレクトリと別のディレクトリにプッシュすることで変更をポーリングして同期を実行します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-117">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="ddb09-118">同期ジョブは、テナントにアプリケーションの特定のインスタンスに固有では常にします。</span><span class="sxs-lookup"><span data-stu-id="ddb09-118">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="ddb09-119">同期ジョブの設定の一部として、ターゲット ディレクトリにオブジェクトを読み書きするための承認を与えると、ジョブの同期スキーマをカスタマイズする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ddb09-119">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="ddb09-120">詳細については、[同期ジョブ](synchronization-synchronizationjob.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddb09-120">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="ddb09-121">同期スキーマ</span><span class="sxs-lookup"><span data-stu-id="ddb09-121">Synchronization schema</span></span>

<span data-ttu-id="ddb09-122">同期スキーマで定義されるオブジェクトの同期し、同期する方法です。</span><span class="sxs-lookup"><span data-stu-id="ddb09-122">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="ddb09-123">同期スキーマには、特定の同期ジョブのセットアップ情報のほとんどが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ddb09-123">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="ddb09-124">通常、[属性マッピング](synchronization-attributemapping.md)の一部をカスタマイズまたはを特定の条件を満たすオブジェクトのみを同期する[スコープのフィルター](synchronization-filter.md)が追加されます。</span><span class="sxs-lookup"><span data-stu-id="ddb09-124">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="ddb09-125">同期スキーマには、次のコンポーネントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ddb09-125">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="ddb09-126">ディレクトリの定義</span><span class="sxs-lookup"><span data-stu-id="ddb09-126">Directory definitions</span></span>
- <span data-ttu-id="ddb09-127">同期ルール</span><span class="sxs-lookup"><span data-stu-id="ddb09-127">Synchronization rules</span></span>
- <span data-ttu-id="ddb09-128">オブジェクトのマッピング</span><span class="sxs-lookup"><span data-stu-id="ddb09-128">Object mappings</span></span>

<span data-ttu-id="ddb09-129">詳細については、[同期スキーマ](synchronization-synchronizationschema.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddb09-129">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="ddb09-130">同期テンプレート</span><span class="sxs-lookup"><span data-stu-id="ddb09-130">Synchronization template</span></span>

<span data-ttu-id="ddb09-131">同期テンプレートは、特定のアプリケーションの構成済みの同期設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-131">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="ddb09-132">(最も重要なは、[同期スキーマ](synchronization-synchronizationschema.md)) は、これらの設定は、テンプレートに基づくすべての[同期ジョブ](synchronization-synchronizationjob.md)の既定で使用されます。</span><span class="sxs-lookup"><span data-stu-id="ddb09-132">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="ddb09-133">テンプレートは、アプリケーション開発者によって指定されます。</span><span class="sxs-lookup"><span data-stu-id="ddb09-133">Templates are specified by the application developer.</span></span>

<span data-ttu-id="ddb09-134">詳細については、[同期のテンプレート](synchronization-synchronizationtemplate.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddb09-134">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="ddb09-135">同期 API を使用します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-135">Working with the synchronization API</span></span>

<span data-ttu-id="ddb09-136">同期を使用する API の主要部分は[synchronizationJob](synchronization-synchronizationjob.md)と[synchronizationSchema](synchronization-synchronizationschema.md)のリソースにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="ddb09-136">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="ddb09-137">[SynchronizationJob](synchronization-synchronizationjob.md)リソースを検索するには、同期ジョブが属するサービスのプリンシパル オブジェクトの ID を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ddb09-137">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="ddb09-138">次の例では、 **synchronizationJob**と**synchronizationSchema**のリソースを操作する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-138">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="ddb09-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddb09-139">Authorization</span></span>

<span data-ttu-id="ddb09-140">Azure AD 同期 API では、OAuth 2.0 を使用して、承認のため。</span><span class="sxs-lookup"><span data-stu-id="ddb09-140">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="ddb09-141">API へのすべての要求を行う前に、アクセス トークンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ddb09-141">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="ddb09-142">詳細については、 [Microsoft Graph を呼び出すための Get アクセス トークン](https://developer.microsoft.com/graph/docs/concepts/auth_overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddb09-142">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="ddb09-143">同期リソースにアクセスするには、アプリケーションには、Directory.ReadWrite.All のアクセス許可が必要があります。</span><span class="sxs-lookup"><span data-stu-id="ddb09-143">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="ddb09-144">詳細については、[ディレクトリのアクセス許可](/graph/permissions-reference#directory-permissions)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddb09-144">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="ddb09-145">サービスのプリンシパル オブジェクトを表示名で検索します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-145">Find the service principal object by display name</span></span>

<span data-ttu-id="ddb09-146">次の例では、表示名でサービスのプリンシパル オブジェクトを検索する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-146">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="ddb09-147">**要求**</span><span class="sxs-lookup"><span data-stu-id="ddb09-147">**Request**</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="ddb09-148">**応答**</span><span class="sxs-lookup"><span data-stu-id="ddb09-148">**Response**</span></span>

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

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="ddb09-149">アプリケーション id サービスのプリンシパル オブジェクトを検索します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-149">Find the service principal object by app ID</span></span>

<span data-ttu-id="ddb09-150">次の使用例は、アプリケーション id サービスのプリンシパル オブジェクトを検索する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ddb09-150">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="ddb09-151">**要求** 
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="ddb09-151">**Request** 
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="ddb09-152">**応答**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="ddb09-152">**Response**
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

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="ddb09-153">既存の同期ジョブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-153">List existing synchronization jobs</span></span>

<span data-ttu-id="ddb09-154">次の使用例は、既存の同期ジョブを一覧表示する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ddb09-154">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="ddb09-155">**要求**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="ddb09-155">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="ddb09-156">**応答**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="ddb09-156">**Response**
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

### <a name="get-synchronization-job-status"></a><span data-ttu-id="ddb09-157">同期ジョブのステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-157">Get synchronization job status</span></span>
<span data-ttu-id="ddb09-158">次の例では、同期ジョブのステータスを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-158">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="ddb09-159">**要求**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="ddb09-159">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="ddb09-160">**応答**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="ddb09-160">**Response**
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

### <a name="get-synchronization-schema"></a><span data-ttu-id="ddb09-161">同期スキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="ddb09-161">Get synchronization schema</span></span>
<span data-ttu-id="ddb09-162">次の例では、同期スキーマを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-162">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="ddb09-163">**要求**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="ddb09-163">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="ddb09-164">**応答**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="ddb09-164">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="ddb09-165">関連項目</span><span class="sxs-lookup"><span data-stu-id="ddb09-165">See also</span></span>

* [<span data-ttu-id="ddb09-166">ディレクトリの拡張属性を使用して同期を構成します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-166">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="ddb09-167">カスタム ターゲットの属性を使用して同期を構成します。</span><span class="sxs-lookup"><span data-stu-id="ddb09-167">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



