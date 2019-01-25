---
title: アプリケーションを更新します。
description: アプリケーション オブジェクトのプロパティを更新します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 335281a0ac37ae3b966f731112223f019a67437d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525949"
---
# <a name="update-application"></a><span data-ttu-id="1d346-103">アプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="1d346-103">Update application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d346-104">アプリケーション オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1d346-104">Update the properties of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d346-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d346-105">Permissions</span></span>
<span data-ttu-id="1d346-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d346-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d346-108">Permission type</span></span>      | <span data-ttu-id="1d346-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d346-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d346-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d346-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1d346-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d346-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d346-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d346-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d346-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d346-113">Not supported.</span></span>    |
|<span data-ttu-id="1d346-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d346-114">Application</span></span> | <span data-ttu-id="1d346-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d346-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d346-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d346-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1d346-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d346-117">Request headers</span></span>
| <span data-ttu-id="1d346-118">名前</span><span class="sxs-lookup"><span data-stu-id="1d346-118">Name</span></span>       | <span data-ttu-id="1d346-119">型</span><span class="sxs-lookup"><span data-stu-id="1d346-119">Type</span></span> | <span data-ttu-id="1d346-120">説明</span><span class="sxs-lookup"><span data-stu-id="1d346-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1d346-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d346-121">Authorization</span></span>  | <span data-ttu-id="1d346-122">string</span><span class="sxs-lookup"><span data-stu-id="1d346-122">string</span></span>  | <span data-ttu-id="1d346-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1d346-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d346-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d346-125">Request body</span></span>
<span data-ttu-id="1d346-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1d346-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1d346-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d346-129">Property</span></span>     | <span data-ttu-id="1d346-130">型</span><span class="sxs-lookup"><span data-stu-id="1d346-130">Type</span></span>   |<span data-ttu-id="1d346-131">説明</span><span class="sxs-lookup"><span data-stu-id="1d346-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d346-132">allowPublicClient</span><span class="sxs-lookup"><span data-stu-id="1d346-132">allowPublicClient</span></span>|<span data-ttu-id="1d346-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="1d346-133">Boolean</span></span>| <span data-ttu-id="1d346-134">アプリケーションは、パブリック クライアントとして動作できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1d346-134">Specifies if the application can act as a public client.</span></span> <span data-ttu-id="1d346-135">たとえば、モバイル デバイスで実行されているインストール済みのアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="1d346-135">For example,  an installed application running on a mobile device.</span></span> <span data-ttu-id="1d346-136">既定値は *false* です。</span><span class="sxs-lookup"><span data-stu-id="1d346-136">Default value is *false*.</span></span> |
|<span data-ttu-id="1d346-137">API</span><span class="sxs-lookup"><span data-stu-id="1d346-137">api</span></span>|<span data-ttu-id="1d346-138">API</span><span class="sxs-lookup"><span data-stu-id="1d346-138">[api](../resources/api.md)</span></span>| <span data-ttu-id="1d346-139">API アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d346-139">Specifies settings for an API application.</span></span> |
|<span data-ttu-id="1d346-140">appRoles</span><span class="sxs-lookup"><span data-stu-id="1d346-140">appRoles</span></span>|<span data-ttu-id="1d346-141">[エンティティ](../resources/approle.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="1d346-141">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="1d346-142">アプリケーションが宣言されているアプリケーション ロールのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1d346-142">The collection of application roles that an application may declare.</span></span> <span data-ttu-id="1d346-143">これらのロールは、ユーザー、グループ、またはサービス ・ プリンシパルを指定できます。</span><span class="sxs-lookup"><span data-stu-id="1d346-143">These roles can be assigned to users, groups, or service principals.</span></span> <span data-ttu-id="1d346-144">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="1d346-144">Not nullable.</span></span>|
|<span data-ttu-id="1d346-145">applicationAliases</span><span class="sxs-lookup"><span data-stu-id="1d346-145">applicationAliases</span></span>|<span data-ttu-id="1d346-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1d346-146">String collection</span></span>| <span data-ttu-id="1d346-147">アプリケーションを識別する Uri。</span><span class="sxs-lookup"><span data-stu-id="1d346-147">The URIs that identify the application.</span></span> <span data-ttu-id="1d346-148">詳細情報は、「[アプリケーションのオブジェクトおよびオブジェクトのサービス プリンシパル](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)です。</span><span class="sxs-lookup"><span data-stu-id="1d346-148">For more information see, [Application Objects and Service Principal Objects](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/).</span></span> <span data-ttu-id="1d346-149">複数値プロパティのフィルター式には *any* 演算子が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d346-149">The *any* operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="1d346-150">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="1d346-150">Not nullable.</span></span> |
|<span data-ttu-id="1d346-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d346-151">createdDateTime</span></span>|<span data-ttu-id="1d346-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d346-152">DateTimeOffset</span></span>| <span data-ttu-id="1d346-153">日付と時刻、アプリケーションが登録されています。</span><span class="sxs-lookup"><span data-stu-id="1d346-153">The date and time the application was registered.</span></span> |
|<span data-ttu-id="1d346-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d346-154">deletedDateTime</span></span>|<span data-ttu-id="1d346-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d346-155">DateTimeOffset</span></span>| <span data-ttu-id="1d346-156">日付と時刻、アプリケーションが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1d346-156">The date and time the application was deleted.</span></span> |
|<span data-ttu-id="1d346-157">displayName</span><span class="sxs-lookup"><span data-stu-id="1d346-157">displayName</span></span>|<span data-ttu-id="1d346-158">String</span><span class="sxs-lookup"><span data-stu-id="1d346-158">String</span></span>|<span data-ttu-id="1d346-159">アプリケーションの表示名です。</span><span class="sxs-lookup"><span data-stu-id="1d346-159">The display name for the application.</span></span> |
|<span data-ttu-id="1d346-160">id</span><span class="sxs-lookup"><span data-stu-id="1d346-160">id</span></span>|<span data-ttu-id="1d346-161">String</span><span class="sxs-lookup"><span data-stu-id="1d346-161">String</span></span>|<span data-ttu-id="1d346-162">アプリケーションの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="1d346-162">The unique identifier for the application.</span></span> <span data-ttu-id="1d346-163">[directoryObject](../resources/directoryobject.md) から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1d346-163">Inherited from [directoryObject](../resources/directoryobject.md).</span></span> <span data-ttu-id="1d346-164">キー。</span><span class="sxs-lookup"><span data-stu-id="1d346-164">Key.</span></span> <span data-ttu-id="1d346-165">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="1d346-165">Not nullable.</span></span> <span data-ttu-id="1d346-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1d346-166">Read-only.</span></span> |
|<span data-ttu-id="1d346-167">Info</span><span class="sxs-lookup"><span data-stu-id="1d346-167">info</span></span>|[<span data-ttu-id="1d346-168">informationalUrl</span><span class="sxs-lookup"><span data-stu-id="1d346-168">informationalUrl</span></span>](../resources/informationalurl.md)| <span data-ttu-id="1d346-169">アプリケーションの基本的なプロファイル情報です。</span><span class="sxs-lookup"><span data-stu-id="1d346-169">Basic profile information of the application.</span></span> | <span data-ttu-id="1d346-170">デスクトップやモバイル デバイスなどのインストールされているクライアントの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d346-170">Specifies settings for installed clients such as desktop or mobile devices.</span></span> |
|<span data-ttu-id="1d346-171">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="1d346-171">keyCredentials</span></span>|<span data-ttu-id="1d346-172">[keyCredential](../resources/keycredential.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1d346-172">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="1d346-173">しないアプリケーションに関連付けられているキーの資格情報のコレクション null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="1d346-173">The collection of key credentials associated with the application Not nullable.</span></span> |
|<span data-ttu-id="1d346-174">logo</span><span class="sxs-lookup"><span data-stu-id="1d346-174">logo</span></span>|<span data-ttu-id="1d346-175">Stream</span><span class="sxs-lookup"><span data-stu-id="1d346-175">Stream</span></span>|<span data-ttu-id="1d346-176">アプリケーションのメインのロゴです。</span><span class="sxs-lookup"><span data-stu-id="1d346-176">The main logo for the application.</span></span> <span data-ttu-id="1d346-177">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="1d346-177">Not nullable.</span></span> |
|<span data-ttu-id="1d346-178">orgRestrictions</span><span class="sxs-lookup"><span data-stu-id="1d346-178">orgRestrictions</span></span>|<span data-ttu-id="1d346-179">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1d346-179">String collection</span></span>| <span data-ttu-id="1d346-180">組織 tenantIds をアプリケーションに制限されます。</span><span class="sxs-lookup"><span data-stu-id="1d346-180">The organizational tenantIds to which the application is restricted.</span></span>  <span data-ttu-id="1d346-181">コレクションが空の場合は、アプリケーションは、マルチ テナント型 (制限されていないです)。</span><span class="sxs-lookup"><span data-stu-id="1d346-181">If the collection is empty, the application is multi-tenant (not restricted).</span></span> <span data-ttu-id="1d346-182">コレクションには、tenantIds が含まれている、アプリケーションは、コレクション内の組織の tenantIds に制限されます。</span><span class="sxs-lookup"><span data-stu-id="1d346-182">If the collection contains tenantIds, the application is restricted to the organizational tenantIds in the collection.</span></span> <span data-ttu-id="1d346-183">他のテナントがアプリケーションが登録されている tenantId ではありませんを指定すると、アプリケーションの tenantId が間接的に含まれていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="1d346-183">Specifying other tenants but not the tenantId where the application is registered implies that the application's own tenantId is indirectly included.</span></span> |
|<span data-ttu-id="1d346-184">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="1d346-184">passwordCredentials</span></span>|<span data-ttu-id="1d346-185">[passwordCredential](../resources/passwordcredential.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1d346-185">[passwordCredential](../resources/passwordcredential.md) collection</span></span>|<span data-ttu-id="1d346-186">アプリケーションに関連付けられているパスワード資格情報のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1d346-186">The collection of password credentials associated with the application.</span></span> <span data-ttu-id="1d346-187">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="1d346-187">Not nullable.</span></span>|
|<span data-ttu-id="1d346-188">preAuthorizedApplications</span><span class="sxs-lookup"><span data-stu-id="1d346-188">preAuthorizedApplications</span></span>|<span data-ttu-id="1d346-189">[preAuthorizedApplication](../resources/preauthorizedapplication.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1d346-189">[preAuthorizedApplication](../resources/preauthorizedapplication.md) collection</span></span>| <span data-ttu-id="1d346-190">アプリケーションと暗黙的な同意を要求されたアクセス許可の一覧です。</span><span class="sxs-lookup"><span data-stu-id="1d346-190">Lists applications and requested permissions for implicit consent.</span></span> <span data-ttu-id="1d346-191">管理者がアプリケーションに同意を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d346-191">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="1d346-192">preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意するものは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="1d346-192">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="1d346-193">PreAuthorizedApplications に記載されているアクセス許可では、ユーザーの同意は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="1d346-193">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="1d346-194">ただし、preAuthorizedApplications に記載されていない追加の要求されたアクセス許可は、ユーザーの同意を必要とします。</span><span class="sxs-lookup"><span data-stu-id="1d346-194">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span> |
|<span data-ttu-id="1d346-195">requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="1d346-195">requiredResourceAccess</span></span>|<span data-ttu-id="1d346-196">[requiredResourceAccess](../resources/requiredresourceaccess.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1d346-196">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span></span>|<span data-ttu-id="1d346-197">このアプリケーションへのアクセスと、OAuth アクセス許可のスコープおよび各リソースの下に必要なアプリケーション ロールのセットを必要とするリソースを指定します。</span><span class="sxs-lookup"><span data-stu-id="1d346-197">Specifies resources that this application requires access to and the set of OAuth permission scopes and application roles that it needs under each of those resources.</span></span> <span data-ttu-id="1d346-198">必要なリソースへのアクセスのこの前の構成では、同意の経験をドライブします。</span><span class="sxs-lookup"><span data-stu-id="1d346-198">This pre-configuration of required resource access drives the consent experience.</span></span> <span data-ttu-id="1d346-199">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="1d346-199">Not nullable.</span></span>|
|<span data-ttu-id="1d346-200">タグの前に追加されるマークアップ</span><span class="sxs-lookup"><span data-stu-id="1d346-200">tags</span></span>|<span data-ttu-id="1d346-201">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1d346-201">String collection</span></span>| <span data-ttu-id="1d346-202">分類し、アプリケーションの識別に使用できるカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="1d346-202">Custom strings that can be used to categorize and identify the application.</span></span> |
|<span data-ttu-id="1d346-203">web</span><span class="sxs-lookup"><span data-stu-id="1d346-203">web</span></span>|<span data-ttu-id="1d346-204">Web</span><span class="sxs-lookup"><span data-stu-id="1d346-204">[web](../resources/web.md)</span></span>| <span data-ttu-id="1d346-205">Web アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d346-205">Specifies settings for a web application.</span></span> |

## <a name="response"></a><span data-ttu-id="1d346-206">応答</span><span class="sxs-lookup"><span data-stu-id="1d346-206">Response</span></span>

<span data-ttu-id="1d346-207">かどうかは成功すると、このメソッドが返されます、`204 No Content`応答コードは、戻り値も、応答の本体で、です。</span><span class="sxs-lookup"><span data-stu-id="1d346-207">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d346-208">例</span><span class="sxs-lookup"><span data-stu-id="1d346-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d346-209">要求</span><span class="sxs-lookup"><span data-stu-id="1d346-209">Request</span></span>
<span data-ttu-id="1d346-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d346-210">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="1d346-211">応答</span><span class="sxs-lookup"><span data-stu-id="1d346-211">Response</span></span>
<span data-ttu-id="1d346-212">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="1d346-212">Note: The response object shown here may be truncated for brevity.</span></span> 
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
    "Error: /api-reference/beta/api/application-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
