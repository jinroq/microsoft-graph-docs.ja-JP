---
title: グループ設定を作成する
description: この API を使用して、groupsettingtemplates で利用可能なテンプレートに基づいて新しい設定を作成します。 これらの設定は、テナントレベルまたはグループレベルで行うことができます。 作成要求では、テンプレートで定義されているすべての設定の settingvalues を指定する必要があります。 グループ固有の設定では、グループのメンバーがゲストユーザーを招待できるかどうかを制御する設定のみが可能です。 これは、グループにゲストユーザーを追加する機能が一般に利用可能になったときに、この動作を制御します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e87e34f5816818c25cef5768c08ab8f7c73a3a0f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577799"
---
# <a name="create-a-group-setting"></a><span data-ttu-id="c8ad5-107">グループ設定を作成する</span><span class="sxs-lookup"><span data-stu-id="c8ad5-107">Create a group setting</span></span>

<span data-ttu-id="c8ad5-p102">この API を使用して、[groupSettingTemplates](../resources/groupsettingtemplate.md) で使用可能なテンプレートに基づいて新しい設定を作成します。これらの設定は、テナント レベルまたはグループ レベルで行うことができます。作成要求は、テンプレートに定義されているすべての設定の [settingValues](../resources/settingvalue.md) を提供する必要があります。グループ固有の設定では、グループのメンバーがゲスト ユーザーを招待できるかどうかの管理のみが設定できます。グループにゲスト ユーザーを追加する機能が一般的に利用可能になると、上記の動作は制御されます。</span><span class="sxs-lookup"><span data-stu-id="c8ad5-p102">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

<span data-ttu-id="c8ad5-113">テンプレートと、それらが v2.0 でサポートするプロパティの一覧については、 [groupsettingtemplate クエリ](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)を使用してください (ベータ版エンドポイントの場合は、call [directorysettingtemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta))。</span><span class="sxs-lookup"><span data-stu-id="c8ad5-113">For a list of templates and the properties they support in v1.0, use a [groupSettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)  (For beta endpoints, call [directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span></span>

## <a name="permissions"></a><span data-ttu-id="c8ad5-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c8ad5-114">Permissions</span></span>

<span data-ttu-id="c8ad5-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8ad5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c8ad5-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8ad5-117">Permission type</span></span>      | <span data-ttu-id="c8ad5-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8ad5-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8ad5-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8ad5-119">Delegated (work or school account)</span></span> | <span data-ttu-id="c8ad5-120">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c8ad5-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c8ad5-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8ad5-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8ad5-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8ad5-122">Not supported.</span></span>    |
|<span data-ttu-id="c8ad5-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8ad5-123">Application</span></span> | <span data-ttu-id="c8ad5-124">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8ad5-124">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8ad5-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8ad5-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="c8ad5-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8ad5-126">Request headers</span></span>

| <span data-ttu-id="c8ad5-127">名前</span><span class="sxs-lookup"><span data-stu-id="c8ad5-127">Name</span></span> | <span data-ttu-id="c8ad5-128">説明</span><span class="sxs-lookup"><span data-stu-id="c8ad5-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c8ad5-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8ad5-129">Authorization</span></span> | <span data-ttu-id="c8ad5-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c8ad5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8ad5-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8ad5-132">Content-Type</span></span> | <span data-ttu-id="c8ad5-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c8ad5-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8ad5-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8ad5-134">Request body</span></span>
<span data-ttu-id="c8ad5-p105">要求本文で、[groupSetting](../resources/groupsetting.md) オブジェクトの JSON 表記を指定します。ただし、設定の表示名は、参照される設定テンプレート名に基づいて設定されます。</span><span class="sxs-lookup"><span data-stu-id="c8ad5-p105">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="c8ad5-137">応答</span><span class="sxs-lookup"><span data-stu-id="c8ad5-137">Response</span></span>

<span data-ttu-id="c8ad5-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [groupSetting](../resources/groupsetting.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8ad5-138">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8ad5-139">例</span><span class="sxs-lookup"><span data-stu-id="c8ad5-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c8ad5-140">要求</span><span class="sxs-lookup"><span data-stu-id="c8ad5-140">Request</span></span>

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
<span data-ttu-id="c8ad5-141">要求本文で、[groupSetting](../resources/groupsetting.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8ad5-141">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c8ad5-142">応答</span><span class="sxs-lookup"><span data-stu-id="c8ad5-142">Response</span></span>

<span data-ttu-id="c8ad5-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c8ad5-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
