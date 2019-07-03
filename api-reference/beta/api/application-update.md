---
title: アプリケーションを更新する
description: Application オブジェクトのプロパティを更新します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dea134cc61e586f94c08755ef812f9f4b7f4e8f7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439596"
---
# <a name="update-application"></a><span data-ttu-id="a6eea-103">アプリケーションを更新する</span><span class="sxs-lookup"><span data-stu-id="a6eea-103">Update application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6eea-104">Application オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a6eea-104">Update the properties of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a6eea-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a6eea-105">Permissions</span></span>
<span data-ttu-id="a6eea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6eea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a6eea-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6eea-108">Permission type</span></span>      | <span data-ttu-id="a6eea-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6eea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6eea-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6eea-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a6eea-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6eea-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a6eea-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6eea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6eea-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6eea-113">Not supported.</span></span>    |
|<span data-ttu-id="a6eea-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6eea-114">Application</span></span> | <span data-ttu-id="a6eea-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6eea-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6eea-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6eea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a6eea-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6eea-117">Request headers</span></span>
| <span data-ttu-id="a6eea-118">名前</span><span class="sxs-lookup"><span data-stu-id="a6eea-118">Name</span></span>       | <span data-ttu-id="a6eea-119">型</span><span class="sxs-lookup"><span data-stu-id="a6eea-119">Type</span></span> | <span data-ttu-id="a6eea-120">説明</span><span class="sxs-lookup"><span data-stu-id="a6eea-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a6eea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6eea-121">Authorization</span></span>  | <span data-ttu-id="a6eea-122">string</span><span class="sxs-lookup"><span data-stu-id="a6eea-122">string</span></span>  | <span data-ttu-id="a6eea-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a6eea-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6eea-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6eea-125">Request body</span></span>
<span data-ttu-id="a6eea-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="a6eea-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a6eea-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6eea-129">Property</span></span>     | <span data-ttu-id="a6eea-130">型</span><span class="sxs-lookup"><span data-stu-id="a6eea-130">Type</span></span>   |<span data-ttu-id="a6eea-131">説明</span><span class="sxs-lookup"><span data-stu-id="a6eea-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6eea-132">allowPublicClient</span><span class="sxs-lookup"><span data-stu-id="a6eea-132">allowPublicClient</span></span>|<span data-ttu-id="a6eea-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6eea-133">Boolean</span></span>| <span data-ttu-id="a6eea-134">アプリケーションがパブリッククライアントとして動作するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a6eea-134">Specifies if the application can act as a public client.</span></span> <span data-ttu-id="a6eea-135">たとえば、モバイルデバイスで実行中のアプリケーションがインストールされている場合です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-135">For example,  an installed application running on a mobile device.</span></span> <span data-ttu-id="a6eea-136">既定値は *false* です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-136">Default value is *false*.</span></span> |
|<span data-ttu-id="a6eea-137">api</span><span class="sxs-lookup"><span data-stu-id="a6eea-137">api</span></span>|[<span data-ttu-id="a6eea-138">apiApplication</span><span class="sxs-lookup"><span data-stu-id="a6eea-138">apiApplication</span></span>](../resources/apiapplication.md)| <span data-ttu-id="a6eea-139">API アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6eea-139">Specifies settings for an API application.</span></span> |
|<span data-ttu-id="a6eea-140">appRoles</span><span class="sxs-lookup"><span data-stu-id="a6eea-140">appRoles</span></span>|<span data-ttu-id="a6eea-141">[appRole](../resources/approle.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6eea-141">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="a6eea-142">アプリケーションで宣言できるアプリケーション ロールのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a6eea-142">The collection of application roles that an application may declare.</span></span> <span data-ttu-id="a6eea-143">これらのロールは、ユーザー、グループ、サービス プリンシパルなどに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="a6eea-143">These roles can be assigned to users, groups, or service principals.</span></span> <span data-ttu-id="a6eea-144">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="a6eea-144">Not nullable.</span></span>|
|<span data-ttu-id="a6eea-145">applicationAliases</span><span class="sxs-lookup"><span data-stu-id="a6eea-145">applicationAliases</span></span>|<span data-ttu-id="a6eea-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a6eea-146">String collection</span></span>| <span data-ttu-id="a6eea-147">アプリケーションを識別する URI です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-147">The URIs that identify the application.</span></span> <span data-ttu-id="a6eea-148">詳細については、「[Azure Active Directory のアプリケーション オブジェクトとサービス プリンシパル オブジェクト](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6eea-148">For more information see, [Application Objects and Service Principal Objects](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/).</span></span> <span data-ttu-id="a6eea-149">複数値プロパティのフィルター式には *any* 演算子が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-149">The *any* operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="a6eea-150">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="a6eea-150">Not nullable.</span></span> |
|<span data-ttu-id="a6eea-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6eea-151">createdDateTime</span></span>|<span data-ttu-id="a6eea-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6eea-152">DateTimeOffset</span></span>| <span data-ttu-id="a6eea-153">アプリケーションが登録された日付と時刻です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-153">The date and time the application was registered.</span></span> |
|<span data-ttu-id="a6eea-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6eea-154">deletedDateTime</span></span>|<span data-ttu-id="a6eea-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6eea-155">DateTimeOffset</span></span>| <span data-ttu-id="a6eea-156">アプリケーションが削除された日付と時刻です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-156">The date and time the application was deleted.</span></span> |
|<span data-ttu-id="a6eea-157">displayName</span><span class="sxs-lookup"><span data-stu-id="a6eea-157">displayName</span></span>|<span data-ttu-id="a6eea-158">String</span><span class="sxs-lookup"><span data-stu-id="a6eea-158">String</span></span>|<span data-ttu-id="a6eea-159">アプリケーションの表示名。</span><span class="sxs-lookup"><span data-stu-id="a6eea-159">The display name for the application.</span></span> |
|<span data-ttu-id="a6eea-160">id</span><span class="sxs-lookup"><span data-stu-id="a6eea-160">id</span></span>|<span data-ttu-id="a6eea-161">String</span><span class="sxs-lookup"><span data-stu-id="a6eea-161">String</span></span>|<span data-ttu-id="a6eea-162">アプリケーションの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-162">The unique identifier for the application.</span></span> <span data-ttu-id="a6eea-163">[directoryObject](../resources/directoryobject.md) から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a6eea-163">Inherited from [directoryObject](../resources/directoryobject.md).</span></span> <span data-ttu-id="a6eea-164">キー。</span><span class="sxs-lookup"><span data-stu-id="a6eea-164">Key.</span></span> <span data-ttu-id="a6eea-165">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="a6eea-165">Not nullable.</span></span> <span data-ttu-id="a6eea-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-166">Read-only.</span></span> |
|<span data-ttu-id="a6eea-167">info</span><span class="sxs-lookup"><span data-stu-id="a6eea-167">info</span></span>|[<span data-ttu-id="a6eea-168">informationalUrl</span><span class="sxs-lookup"><span data-stu-id="a6eea-168">informationalUrl</span></span>](../resources/informationalurl.md)| <span data-ttu-id="a6eea-169">アプリケーションの基本的なプロファイル情報です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-169">Basic profile information of the application.</span></span> | <span data-ttu-id="a6eea-170">デスクトップやモバイル デバイスなど、インストールされているクライアントの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6eea-170">Specifies settings for installed clients such as desktop or mobile devices.</span></span> |
|<span data-ttu-id="a6eea-171">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="a6eea-171">keyCredentials</span></span>|<span data-ttu-id="a6eea-172">[keyCredential](../resources/keycredential.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6eea-172">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="a6eea-173">アプリケーションに関連付けられているキー資格情報のコレクションです。null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="a6eea-173">The collection of key credentials associated with the application Not nullable.</span></span> |
|<span data-ttu-id="a6eea-174">logo</span><span class="sxs-lookup"><span data-stu-id="a6eea-174">logo</span></span>|<span data-ttu-id="a6eea-175">Stream</span><span class="sxs-lookup"><span data-stu-id="a6eea-175">Stream</span></span>|<span data-ttu-id="a6eea-176">アプリケーションのメイン ロゴです。</span><span class="sxs-lookup"><span data-stu-id="a6eea-176">The main logo for the application.</span></span> <span data-ttu-id="a6eea-177">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="a6eea-177">Not nullable.</span></span> |
|<span data-ttu-id="a6eea-178">orgRestrictions</span><span class="sxs-lookup"><span data-stu-id="a6eea-178">orgRestrictions</span></span>|<span data-ttu-id="a6eea-179">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a6eea-179">String collection</span></span>| <span data-ttu-id="a6eea-180">アプリケーションが制限されている組織の整理された Ds。</span><span class="sxs-lookup"><span data-stu-id="a6eea-180">The organizational tenantIds to which the application is restricted.</span></span>  <span data-ttu-id="a6eea-181">コレクションが空の場合、アプリケーションはマルチテナント (制限なし) です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-181">If the collection is empty, the application is multi-tenant (not restricted).</span></span> <span data-ttu-id="a6eea-182">コレクションに保持されている Ds がある場合、アプリケーションはコレクション内の整理された Ds に制限されます。</span><span class="sxs-lookup"><span data-stu-id="a6eea-182">If the collection contains tenantIds, the application is restricted to the organizational tenantIds in the collection.</span></span> <span data-ttu-id="a6eea-183">アプリケーションが登録されている tenantId を指定せずに他のテナントを指定すると、アプリケーション自体の tenantId が間接的に含まれていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="a6eea-183">Specifying other tenants but not the tenantId where the application is registered implies that the application's own tenantId is indirectly included.</span></span> |
|<span data-ttu-id="a6eea-184">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="a6eea-184">passwordCredentials</span></span>|<span data-ttu-id="a6eea-185">[passwordCredential](../resources/passwordcredential.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6eea-185">[passwordCredential](../resources/passwordcredential.md) collection</span></span>|<span data-ttu-id="a6eea-186">アプリケーションに関連付けられているパスワード資格情報のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a6eea-186">The collection of password credentials associated with the application.</span></span> <span data-ttu-id="a6eea-187">null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="a6eea-187">Not nullable.</span></span>|
|<span data-ttu-id="a6eea-188">preAuthorizedApplications</span><span class="sxs-lookup"><span data-stu-id="a6eea-188">preAuthorizedApplications</span></span>|<span data-ttu-id="a6eea-189">[Preauthorizedapplication](../resources/preauthorizedapplication.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a6eea-189">[preAuthorizedApplication](../resources/preauthorizedapplication.md) collection</span></span>| <span data-ttu-id="a6eea-190">アプリケーションおよび暗黙的同意の要求されたアクセス許可を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a6eea-190">Lists applications and requested permissions for implicit consent.</span></span> <span data-ttu-id="a6eea-191">管理者はアプリケーションに同意を得る必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6eea-191">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="a6eea-192">preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a6eea-192">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="a6eea-193">PreAuthorizedApplications にリストされているアクセス許可は、ユーザーの同意を必要としません。</span><span class="sxs-lookup"><span data-stu-id="a6eea-193">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="a6eea-194">ただし、preAuthorizedApplications に表示されていない追加の要求されたアクセス許可には、ユーザーの同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-194">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span> |
|<span data-ttu-id="a6eea-195">requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="a6eea-195">requiredResourceAccess</span></span>|<span data-ttu-id="a6eea-196">[requiredResourceAccess](../resources/requiredresourceaccess.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6eea-196">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span></span>|<span data-ttu-id="a6eea-197">このアプリケーションがアクセスする必要があるリソース、およびそのリソースで必要な OAuth アクセス許可の範囲とアプリケーション ロールのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="a6eea-197">Specifies resources that this application requires access to and the set of OAuth permission scopes and application roles that it needs under each of those resources.</span></span> <span data-ttu-id="a6eea-198">必要なリソースへのアクセスに対するこの事前構成によって、同意エクスペリエンスが促進されます。</span><span class="sxs-lookup"><span data-stu-id="a6eea-198">This pre-configuration of required resource access drives the consent experience.</span></span> <span data-ttu-id="a6eea-199">null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="a6eea-199">Not nullable.</span></span>|
|<span data-ttu-id="a6eea-200">tags</span><span class="sxs-lookup"><span data-stu-id="a6eea-200">tags</span></span>|<span data-ttu-id="a6eea-201">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a6eea-201">String collection</span></span>| <span data-ttu-id="a6eea-202">アプリケーションを分類および識別するために使用できるカスタム文字列です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-202">Custom strings that can be used to categorize and identify the application.</span></span> |
|<span data-ttu-id="a6eea-203">Web</span><span class="sxs-lookup"><span data-stu-id="a6eea-203">web</span></span>|[<span data-ttu-id="a6eea-204">webApplication</span><span class="sxs-lookup"><span data-stu-id="a6eea-204">webApplication</span></span>](../resources/webapplication.md)| <span data-ttu-id="a6eea-205">Web アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6eea-205">Specifies settings for a web application.</span></span> |

## <a name="response"></a><span data-ttu-id="a6eea-206">応答</span><span class="sxs-lookup"><span data-stu-id="a6eea-206">Response</span></span>

<span data-ttu-id="a6eea-207">成功した場合、このメソッド`204 No Content`は応答コードを返し、応答本文では何も返しません。</span><span class="sxs-lookup"><span data-stu-id="a6eea-207">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6eea-208">例</span><span class="sxs-lookup"><span data-stu-id="a6eea-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6eea-209">要求</span><span class="sxs-lookup"><span data-stu-id="a6eea-209">Request</span></span>
<span data-ttu-id="a6eea-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6eea-210">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a6eea-211">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a6eea-211">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json
Content-length: 72

{
  "allowPublicClient": false,
  "displayName": "New display name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a6eea-212">C#</span><span class="sxs-lookup"><span data-stu-id="a6eea-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6eea-213">Javascript</span><span class="sxs-lookup"><span data-stu-id="a6eea-213">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a6eea-214">目的-C</span><span class="sxs-lookup"><span data-stu-id="a6eea-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a6eea-215">応答</span><span class="sxs-lookup"><span data-stu-id="a6eea-215">Response</span></span>
<span data-ttu-id="a6eea-216">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a6eea-216">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
