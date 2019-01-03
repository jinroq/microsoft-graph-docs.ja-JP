---
title: グループ設定を更新する
description: 特定のグループ設定オブジェクトのプロパティを更新します。
author: dkershaw10
ms.openlocfilehash: 07ab3114ce4ed5d8d932ff9183c62823ddfcf632
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339838"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="84937-103">グループ設定を更新する</span><span class="sxs-lookup"><span data-stu-id="84937-103">Update a group setting</span></span>

<span data-ttu-id="84937-104">特定のグループ設定オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="84937-104">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84937-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="84937-105">Permissions</span></span>

<span data-ttu-id="84937-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84937-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="84937-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84937-108">Permission type</span></span>      | <span data-ttu-id="84937-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="84937-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84937-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84937-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84937-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="84937-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="84937-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84937-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84937-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84937-113">Not supported.</span></span>    |
|<span data-ttu-id="84937-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84937-114">Application</span></span> | <span data-ttu-id="84937-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84937-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84937-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84937-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="84937-117">テナント全体またはグループ固有の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="84937-117">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="84937-118">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84937-118">Optional request headers</span></span>
| <span data-ttu-id="84937-119">名前</span><span class="sxs-lookup"><span data-stu-id="84937-119">Name</span></span> | <span data-ttu-id="84937-120">説明</span><span class="sxs-lookup"><span data-stu-id="84937-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="84937-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="84937-121">Authorization</span></span>  | <span data-ttu-id="84937-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="84937-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84937-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84937-124">Content-Type</span></span>  | <span data-ttu-id="84937-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84937-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="84937-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="84937-126">Request body</span></span>
<span data-ttu-id="84937-127">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="84937-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="84937-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84937-128">Property</span></span> | <span data-ttu-id="84937-129">種類</span><span class="sxs-lookup"><span data-stu-id="84937-129">Type</span></span> | <span data-ttu-id="84937-130">説明</span><span class="sxs-lookup"><span data-stu-id="84937-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="84937-131">values</span><span class="sxs-lookup"><span data-stu-id="84937-131">values</span></span> | <span data-ttu-id="84937-132">settingValue コレクション</span><span class="sxs-lookup"><span data-stu-id="84937-132">settingValue collection</span></span> | <span data-ttu-id="84937-p103">更新された値のセットです。注:コレクション セット全体を指定する必要があります。単一の値のセットを更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="84937-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="84937-136">応答</span><span class="sxs-lookup"><span data-stu-id="84937-136">Response</span></span>

<span data-ttu-id="84937-137">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="84937-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="84937-138">例</span><span class="sxs-lookup"><span data-stu-id="84937-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="84937-139">要求</span><span class="sxs-lookup"><span data-stu-id="84937-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "CustomBlockedWordsList",
      "value": ""
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "False"
    },
    {
      "name": "ClassificationDescriptions",
      "value": ""
    },
    {
      "name": "DefaultClassification",
      "value": ""
    },
    {
      "name": "PrefixSuffixNamingRequirement",
      "value": ""
    },
    {
      "name": "AllowGuestsToBeGroupOwner",
      "value": "False"
    },
    {
      "name": "AllowGuestsToAccessGroups",
      "value": "True"
    },
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "GroupCreationAllowedGroupId",
      "value": "62e90394-69f5-4237-9190-012177145e10"
    },
    {
      "name": "AllowToAddGuests",
      "value": "True"
    },
    {
      "name": "UsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "ClassificationList",
      "value": ""
    },
    {
      "name": "EnableGroupCreation",
      "value": "True"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="84937-140">応答</span><span class="sxs-lookup"><span data-stu-id="84937-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->