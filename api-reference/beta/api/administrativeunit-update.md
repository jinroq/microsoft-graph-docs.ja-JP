---
title: Administrativeunit を更新します。
description: AdministrativeUnit オブジェクトのプロパティを更新します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cd82035e06fbd6135f4d2f6cbb7f6dfae9576f9a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932015"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="d73de-103">Administrativeunit を更新します。</span><span class="sxs-lookup"><span data-stu-id="d73de-103">Update administrativeunit</span></span>

> <span data-ttu-id="d73de-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d73de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d73de-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d73de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d73de-106">[AdministrativeUnit](../resources/administrativeunit.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d73de-106">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d73de-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d73de-107">Permissions</span></span>
<span data-ttu-id="d73de-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d73de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d73de-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d73de-110">Permission type</span></span>      | <span data-ttu-id="d73de-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d73de-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d73de-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d73de-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d73de-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d73de-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d73de-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d73de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d73de-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d73de-115">Not supported.</span></span>    |
|<span data-ttu-id="d73de-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d73de-116">Application</span></span> | <span data-ttu-id="d73de-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d73de-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d73de-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d73de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d73de-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d73de-119">Request headers</span></span>

| <span data-ttu-id="d73de-120">名前</span><span class="sxs-lookup"><span data-stu-id="d73de-120">Name</span></span>      |<span data-ttu-id="d73de-121">説明</span><span class="sxs-lookup"><span data-stu-id="d73de-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d73de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d73de-122">Authorization</span></span>  | <span data-ttu-id="d73de-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d73de-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d73de-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d73de-125">Request body</span></span>

<span data-ttu-id="d73de-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="d73de-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d73de-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d73de-129">Property</span></span>   | <span data-ttu-id="d73de-130">種類</span><span class="sxs-lookup"><span data-stu-id="d73de-130">Type</span></span> |<span data-ttu-id="d73de-131">説明</span><span class="sxs-lookup"><span data-stu-id="d73de-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d73de-132">description</span><span class="sxs-lookup"><span data-stu-id="d73de-132">description</span></span>|<span data-ttu-id="d73de-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d73de-133">string</span></span>|<span data-ttu-id="d73de-134">管理単位の説明です。</span><span class="sxs-lookup"><span data-stu-id="d73de-134">Description for the administrative unit.</span></span>|
|<span data-ttu-id="d73de-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d73de-135">displayName</span></span>|<span data-ttu-id="d73de-136">string</span><span class="sxs-lookup"><span data-stu-id="d73de-136">string</span></span>|<span data-ttu-id="d73de-137">管理単位の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="d73de-137">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="d73de-138">visibility</span><span class="sxs-lookup"><span data-stu-id="d73de-138">visibility</span></span>|<span data-ttu-id="d73de-139">文字列</span><span class="sxs-lookup"><span data-stu-id="d73de-139">string</span></span>|<span data-ttu-id="d73de-140">管理単位の表示/非表示にします。</span><span class="sxs-lookup"><span data-stu-id="d73de-140">Visibility for the administrative unit.</span></span> <span data-ttu-id="d73de-141">設定されていない場合、既定値はパブリックです。</span><span class="sxs-lookup"><span data-stu-id="d73de-141">If not set then the default is "public".</span></span> <span data-ttu-id="d73de-142">"HiddenMembership"は、メンバー以外のメンバーのメンバーシップを非表示にするに設定することができます。</span><span class="sxs-lookup"><span data-stu-id="d73de-142">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="d73de-143">使用することができます**administrativeUnit**リソースでは、[拡張機能](/graph/extensibility-overview)をサポートするため、`PATCH`を追加、更新、または既存の**administrativeUnit**インスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="d73de-143">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="d73de-144">応答</span><span class="sxs-lookup"><span data-stu-id="d73de-144">Response</span></span>

<span data-ttu-id="d73de-145">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d73de-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d73de-146">例</span><span class="sxs-lookup"><span data-stu-id="d73de-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d73de-147">要求</span><span class="sxs-lookup"><span data-stu-id="d73de-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/beta/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```

##### <a name="response"></a><span data-ttu-id="d73de-148">応答</span><span class="sxs-lookup"><span data-stu-id="d73de-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="d73de-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="d73de-149">See also</span></span>

- [<span data-ttu-id="d73de-150">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="d73de-150">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d73de-151">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="d73de-151">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
