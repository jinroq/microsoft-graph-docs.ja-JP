# <a name="force-domain-deletion"></a><span data-ttu-id="4009b-101">強制的にドメインの削除</span><span class="sxs-lookup"><span data-stu-id="4009b-101">Force domain deletion</span></span>

<span data-ttu-id="4009b-102">非同期実行時間の長い操作を使用してドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="4009b-102">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="4009b-103">次の操作は、この操作の一部として実行されます。</span><span class="sxs-lookup"><span data-stu-id="4009b-103">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="4009b-104">更新、 `userPrincipalName`、 `mail`、および`proxyAddresses`のプロパティ`users`初期 onmicrosoft.com ドメインを使用する削除されたドメインへの参照にします。</span><span class="sxs-lookup"><span data-stu-id="4009b-104">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="4009b-105">更新、`mail`の`groups`初期 onmicrosoft.com ドメインを使用する削除されたドメインへの参照にします。</span><span class="sxs-lookup"><span data-stu-id="4009b-105">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="4009b-106">更新、`identifierUris`の`applications`初期 onmicrosoft.com ドメインを使用する削除されたドメインへの参照にします。</span><span class="sxs-lookup"><span data-stu-id="4009b-106">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="4009b-107">名前を変更するオブジェクトの数が 1000 を超える場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="4009b-107">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="4009b-108">1 つの場合の`applications`は、マルチ テナント アプリケーションの名前を変更するのには、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="4009b-108">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="4009b-109">ドメインの削除が完了すると、削除されたドメインの API 操作は HTTP 404 ステータス コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4009b-109">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="4009b-110">ドメインの削除を確認するには、[ドメインの取得](domain_get.md)の操作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="4009b-110">To verify deletion of a domain, you can perform a [get domain](domain_get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="4009b-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4009b-111">Permissions</span></span>

<span data-ttu-id="4009b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4009b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4009b-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4009b-114">Permission type</span></span>      | <span data-ttu-id="4009b-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4009b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4009b-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4009b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4009b-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4009b-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4009b-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4009b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4009b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4009b-119">Not supported.</span></span>    |
|<span data-ttu-id="4009b-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4009b-120">Application</span></span> | <span data-ttu-id="4009b-121">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4009b-121">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4009b-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4009b-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="4009b-123">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="4009b-123">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4009b-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4009b-124">Request headers</span></span>

| <span data-ttu-id="4009b-125">名前</span><span class="sxs-lookup"><span data-stu-id="4009b-125">Name</span></span> | <span data-ttu-id="4009b-126">説明</span><span class="sxs-lookup"><span data-stu-id="4009b-126">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4009b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4009b-127">Authorization</span></span>  | <span data-ttu-id="4009b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4009b-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4009b-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4009b-130">Content-Type</span></span>  | <span data-ttu-id="4009b-131">application/json</span><span class="sxs-lookup"><span data-stu-id="4009b-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4009b-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="4009b-132">Request body</span></span>

<span data-ttu-id="4009b-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="4009b-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4009b-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4009b-134">Parameter</span></span> | <span data-ttu-id="4009b-135">型</span><span class="sxs-lookup"><span data-stu-id="4009b-135">Type</span></span> | <span data-ttu-id="4009b-136">説明</span><span class="sxs-lookup"><span data-stu-id="4009b-136">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="4009b-137">名前を変更するユーザー アカウントを無効にするオプションです。</span><span class="sxs-lookup"><span data-stu-id="4009b-137">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="4009b-138">ユーザー アカウントを無効にすると、ユーザーはサインインするのには使用できません。</span><span class="sxs-lookup"><span data-stu-id="4009b-138">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="4009b-139">場合**は true**に設定、`users`この操作の一部が無効にするたびに更新します。</span><span class="sxs-lookup"><span data-stu-id="4009b-139">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="4009b-140">既定値は**true**です。</span><span class="sxs-lookup"><span data-stu-id="4009b-140">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="4009b-141">応答本文</span><span class="sxs-lookup"><span data-stu-id="4009b-141">Response body</span></span>

<span data-ttu-id="4009b-142">かどうかは成功すると、このメソッドを返します`HTTP/1.1 204 OK`ステータス コードです。</span><span class="sxs-lookup"><span data-stu-id="4009b-142">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="4009b-143">例</span><span class="sxs-lookup"><span data-stu-id="4009b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4009b-144">要求</span><span class="sxs-lookup"><span data-stu-id="4009b-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

### <a name="response"></a><span data-ttu-id="4009b-145">応答</span><span class="sxs-lookup"><span data-stu-id="4009b-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->