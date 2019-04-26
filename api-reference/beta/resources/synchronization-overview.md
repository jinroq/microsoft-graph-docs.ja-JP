---
title: Azure AD 同期 API の概要
description: ) を使用すると、削除、管理、およびクラウドでの id の作成、保守、および削除 (たとえば、サービスとしてのソフトウェア、または SaaS) アプリケーション (Dropbox、Salesforce、ServiceNow など) を自動化できます。 Microsoft Graph の同期 api を使用して、次のようなプログラムによって id 同期を管理できます。
localization_priority: Normal
ms.openlocfilehash: e472acc60e74c6a22a744d84e7e4dcf672337a6e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342930"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="79732-104">Azure AD 同期 API の概要</span><span class="sxs-lookup"><span data-stu-id="79732-104">Azure AD synchronization API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79732-105">azure Active Directory (azure AD) id 同期 ("プロビジョニング" とも呼ばれます) により、(サービスとしてのソフトウェア、または SaaS) アプリケーションとしての、クラウドでの id の作成、保守、削除を自動化できます (Dropbox、Salesforce、ServiceNow、その他。</span><span class="sxs-lookup"><span data-stu-id="79732-105">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="79732-106">Microsoft Graph の同期 api を使用して、次のようなプログラムによって id 同期を管理できます。</span><span class="sxs-lookup"><span data-stu-id="79732-106">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="79732-107">同期ジョブの作成、開始、停止</span><span class="sxs-lookup"><span data-stu-id="79732-107">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="79732-108">ジョブの同期スキーマに変更を加える</span><span class="sxs-lookup"><span data-stu-id="79732-108">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="79732-109">現在の同期の状態を確認する</span><span class="sxs-lookup"><span data-stu-id="79732-109">Verify the current synchronization status</span></span> 

<span data-ttu-id="79732-110">Azure AD での同期の詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79732-110">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="79732-111">Azure Active Directory を使用した SaaS アプリケーションへのユーザープロビジョニングとプロビジョニング解除を自動化する</span><span class="sxs-lookup"><span data-stu-id="79732-111">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="79732-112">Azure portal でエンタープライズアプリのユーザーアカウントプロビジョニングを管理する</span><span class="sxs-lookup"><span data-stu-id="79732-112">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="79732-113">サンプルテナントまたは独自のテナントで、 [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API を試すこともできます。</span><span class="sxs-lookup"><span data-stu-id="79732-113">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="79732-114">同期ジョブ</span><span class="sxs-lookup"><span data-stu-id="79732-114">Synchronization job</span></span>

<span data-ttu-id="79732-115">同期ジョブは、バックグラウンドで定期的に実行して同期を実行し、1つのディレクトリに加えられた変更をポーリングして、別のディレクトリにプッシュします。</span><span class="sxs-lookup"><span data-stu-id="79732-115">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="79732-116">同期ジョブは、テナント内のアプリケーションの特定のインスタンスに対して常に固有です。</span><span class="sxs-lookup"><span data-stu-id="79732-116">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="79732-117">同期ジョブの設定の一部として、ターゲットディレクトリのオブジェクトの読み取りおよび書き込みの承認を付与し、ジョブの同期スキーマをカスタマイズする必要があります。</span><span class="sxs-lookup"><span data-stu-id="79732-117">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="79732-118">詳細については、「[同期ジョブ](synchronization-synchronizationjob.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79732-118">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="79732-119">同期スキーマ</span><span class="sxs-lookup"><span data-stu-id="79732-119">Synchronization schema</span></span>

<span data-ttu-id="79732-120">同期スキーマは、どのオブジェクトが同期されるか、またどのように同期されるかを定義します。</span><span class="sxs-lookup"><span data-stu-id="79732-120">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="79732-121">同期スキーマには、特定の同期ジョブの設定情報の大部分が含まれています。</span><span class="sxs-lookup"><span data-stu-id="79732-121">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="79732-122">通常、[属性マッピング](synchronization-attributemapping.md)の一部をカスタマイズするか、特定の条件を満たすオブジェクトのみを同期する[スコープフィルター](synchronization-filter.md)を追加します。</span><span class="sxs-lookup"><span data-stu-id="79732-122">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="79732-123">同期スキーマには、次のコンポーネントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="79732-123">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="79732-124">ディレクトリ定義</span><span class="sxs-lookup"><span data-stu-id="79732-124">Directory definitions</span></span>
- <span data-ttu-id="79732-125">同期ルール</span><span class="sxs-lookup"><span data-stu-id="79732-125">Synchronization rules</span></span>
- <span data-ttu-id="79732-126">オブジェクトマッピング</span><span class="sxs-lookup"><span data-stu-id="79732-126">Object mappings</span></span>

<span data-ttu-id="79732-127">詳細については、「[同期スキーマ](synchronization-synchronizationschema.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79732-127">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="79732-128">同期テンプレート</span><span class="sxs-lookup"><span data-stu-id="79732-128">Synchronization template</span></span>

<span data-ttu-id="79732-129">同期テンプレートは、特定のアプリケーションに事前に構成された同期設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="79732-129">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="79732-130">これらの設定 (最も重要なのは[同期スキーマ](synchronization-synchronizationschema.md)) は、テンプレートに基づくすべての[同期ジョブ](synchronization-synchronizationjob.md)に対して既定で使用されます。</span><span class="sxs-lookup"><span data-stu-id="79732-130">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="79732-131">テンプレートは、アプリケーション開発者によって指定されます。</span><span class="sxs-lookup"><span data-stu-id="79732-131">Templates are specified by the application developer.</span></span>

<span data-ttu-id="79732-132">詳細については、「[同期テンプレート](synchronization-synchronizationtemplate.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79732-132">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="79732-133">同期 API を使用する</span><span class="sxs-lookup"><span data-stu-id="79732-133">Working with the synchronization API</span></span>

<span data-ttu-id="79732-134">同期 API の処理では、主に同期[ジョブ](synchronization-synchronizationjob.md)と同期[スキーマ](synchronization-synchronizationschema.md)リソースにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="79732-134">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="79732-135">同期[ジョブ](synchronization-synchronizationjob.md)リソースを見つけるには、同期ジョブが属するサービスプリンシパルオブジェクトの ID を知る必要があります。</span><span class="sxs-lookup"><span data-stu-id="79732-135">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="79732-136">次の例は、**同期ジョブ**と**同期スキーマ**リソースを操作する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="79732-136">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="79732-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="79732-137">Authorization</span></span>

<span data-ttu-id="79732-138">Azure AD 同期 API は、認証に OAuth 2.0 を使用します。</span><span class="sxs-lookup"><span data-stu-id="79732-138">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="79732-139">API に対して要求を行う前に、アクセストークンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="79732-139">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="79732-140">詳細については、「 [Microsoft Graph を呼び出すためのアクセストークンの取得](https://developer.microsoft.com/graph/docs/concepts/auth_overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79732-140">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="79732-141">同期リソースにアクセスするには、アプリケーションにディレクトリの ReadWrite というアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="79732-141">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="79732-142">詳細については、「[ディレクトリのアクセス許可](/graph/permissions-reference#directory-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79732-142">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="79732-143">表示名でサービスプリンシパルオブジェクトを検索する</span><span class="sxs-lookup"><span data-stu-id="79732-143">Find the service principal object by display name</span></span>

<span data-ttu-id="79732-144">次の例は、表示名でサービスプリンシパルオブジェクトを検索する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="79732-144">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="79732-145">**要求**</span><span class="sxs-lookup"><span data-stu-id="79732-145">**Request**</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="79732-146">**応答**</span><span class="sxs-lookup"><span data-stu-id="79732-146">**Response**</span></span>

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

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="79732-147">サービスプリンシパルオブジェクトをアプリ ID で検索する</span><span class="sxs-lookup"><span data-stu-id="79732-147">Find the service principal object by app ID</span></span>

<span data-ttu-id="79732-148">次の例は、サービスプリンシパルオブジェクトをアプリ ID で検索する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="79732-148">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="79732-149">**タキ** 
</span><span class="sxs-lookup"><span data-stu-id="79732-149">**Request** 
</span></span><!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="79732-150">**応答**</span><span class="sxs-lookup"><span data-stu-id="79732-150">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
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

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="79732-151">既存の同期ジョブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="79732-151">List existing synchronization jobs</span></span>

<span data-ttu-id="79732-152">次の例は、既存の同期ジョブを一覧表示する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="79732-152">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="79732-153">**要求**</span><span class="sxs-lookup"><span data-stu-id="79732-153">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="79732-154">**応答**</span><span class="sxs-lookup"><span data-stu-id="79732-154">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
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

### <a name="get-synchronization-job-status"></a><span data-ttu-id="79732-155">同期ジョブの状態を取得する</span><span class="sxs-lookup"><span data-stu-id="79732-155">Get synchronization job status</span></span>
<span data-ttu-id="79732-156">次の例は、同期ジョブの状態を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="79732-156">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="79732-157">**要求**</span><span class="sxs-lookup"><span data-stu-id="79732-157">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="79732-158">**応答**</span><span class="sxs-lookup"><span data-stu-id="79732-158">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
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

### <a name="get-synchronization-schema"></a><span data-ttu-id="79732-159">同期スキーマを取得する</span><span class="sxs-lookup"><span data-stu-id="79732-159">Get synchronization schema</span></span>
<span data-ttu-id="79732-160">次の例は、同期スキーマを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="79732-160">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="79732-161">**要求**</span><span class="sxs-lookup"><span data-stu-id="79732-161">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="79732-162">**応答**</span><span class="sxs-lookup"><span data-stu-id="79732-162">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="79732-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="79732-163">See also</span></span>

* [<span data-ttu-id="79732-164">ディレクトリ拡張属性を使用して同期を構成する</span><span class="sxs-lookup"><span data-stu-id="79732-164">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="79732-165">カスタムターゲット属性を使用して同期を構成する</span><span class="sxs-lookup"><span data-stu-id="79732-165">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



