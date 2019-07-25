---
title: グループ設定を作成する
description: この API を使用して、groupSettingTemplates で利用可能なテンプレートに基づいて新しい設定を作成します。 これらの設定は、テナントレベルまたはグループレベルで行うことができます。 作成要求では、テンプレートで定義されているすべての設定の settingValues を指定する必要があります。 グループ固有の設定では、グループのメンバーがゲストユーザーを招待できるかどうかを制御する設定のみが可能です。 これは、グループにゲストユーザーを追加する機能が一般に利用可能になったときに、この動作を制御します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 362de1245d41f849e940a3e6e87b42ffbffac522
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884120"
---
# <a name="create-a-group-setting"></a><span data-ttu-id="ae084-107">グループ設定を作成する</span><span class="sxs-lookup"><span data-stu-id="ae084-107">Create a group setting</span></span>

<span data-ttu-id="ae084-p102">この API を使用して、[groupSettingTemplates](../resources/groupsettingtemplate.md) で使用可能なテンプレートに基づいて新しい設定を作成します。これらの設定は、テナント レベルまたはグループ レベルで行うことができます。作成要求は、テンプレートに定義されているすべての設定の [settingValues](../resources/settingvalue.md) を提供する必要があります。グループ固有の設定では、グループのメンバーがゲスト ユーザーを招待できるかどうかの管理のみが設定できます。グループにゲスト ユーザーを追加する機能が一般的に利用可能になると、上記の動作は制御されます。</span><span class="sxs-lookup"><span data-stu-id="ae084-p102">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

<span data-ttu-id="ae084-113">テンプレートと、それらが v2.0 でサポートするプロパティの一覧については、 [Groupsettingtemplate クエリ](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)を使用してください (ベータ版エンドポイントの場合は、Call [directorysettingtemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta))。</span><span class="sxs-lookup"><span data-stu-id="ae084-113">For a list of templates and the properties they support in v1.0, use a [groupSettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)  (For beta endpoints, call [directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span></span>

## <a name="permissions"></a><span data-ttu-id="ae084-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae084-114">Permissions</span></span>

<span data-ttu-id="ae084-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae084-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ae084-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae084-117">Permission type</span></span>      | <span data-ttu-id="ae084-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae084-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae084-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae084-119">Delegated (work or school account)</span></span> | <span data-ttu-id="ae084-120">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae084-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae084-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae084-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae084-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae084-122">Not supported.</span></span>    |
|<span data-ttu-id="ae084-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae084-123">Application</span></span> | <span data-ttu-id="ae084-124">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae084-124">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae084-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae084-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="ae084-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae084-126">Request headers</span></span>

| <span data-ttu-id="ae084-127">名前</span><span class="sxs-lookup"><span data-stu-id="ae084-127">Name</span></span> | <span data-ttu-id="ae084-128">説明</span><span class="sxs-lookup"><span data-stu-id="ae084-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ae084-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae084-129">Authorization</span></span> | <span data-ttu-id="ae084-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae084-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae084-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae084-132">Content-Type</span></span> | <span data-ttu-id="ae084-133">application/json</span><span class="sxs-lookup"><span data-stu-id="ae084-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae084-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae084-134">Request body</span></span>
<span data-ttu-id="ae084-p105">要求本文で、[groupSetting](../resources/groupsetting.md) オブジェクトの JSON 表記を指定します。ただし、設定の表示名は、参照される設定テンプレート名に基づいて設定されます。</span><span class="sxs-lookup"><span data-stu-id="ae084-p105">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="ae084-137">応答</span><span class="sxs-lookup"><span data-stu-id="ae084-137">Response</span></span>

<span data-ttu-id="ae084-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [groupSetting](../resources/groupsetting.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ae084-138">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae084-139">例</span><span class="sxs-lookup"><span data-stu-id="ae084-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ae084-140">要求</span><span class="sxs-lookup"><span data-stu-id="ae084-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ae084-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ae084-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ae084-142">C#</span><span class="sxs-lookup"><span data-stu-id="ae084-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-groupsetting-from-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae084-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="ae084-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ae084-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="ae084-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ae084-145">Java</span><span class="sxs-lookup"><span data-stu-id="ae084-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ae084-146">要求本文で、[groupSetting](../resources/groupsetting.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae084-146">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ae084-147">応答</span><span class="sxs-lookup"><span data-stu-id="ae084-147">Response</span></span>

<span data-ttu-id="ae084-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae084-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 238

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
