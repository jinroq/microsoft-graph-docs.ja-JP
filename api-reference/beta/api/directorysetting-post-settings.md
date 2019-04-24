---
title: ディレクトリ設定を作成する
description: この API を使用して、directorysettingtemplates で利用可能なテンプレートに基づいて新しい設定を作成します。 これらの設定は、テナントレベルまたはオブジェクトレベルで行うことができます (現在はグループに対してのみ)。 作成要求では、テンプレートで定義されているすべての設定の settingvalues を指定する必要があります。 グループ固有の設定では、グループのメンバーがゲストユーザーを招待できるかどうかを制御する設定のみが可能です。 これは、グループにゲストユーザーを追加する機能が一般に利用可能になったときに、この動作を制御します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f74c449f02726adc4ba0993f450a8a4351ec8f2a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454891"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="2fc7d-107">ディレクトリ設定を作成する</span><span class="sxs-lookup"><span data-stu-id="2fc7d-107">Create a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fc7d-108">この API を使用して、directorysettingtemplates で利用可能なテンプレートに基づいて新しい設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-108">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="2fc7d-109">これらの設定は、テナントレベルまたはオブジェクトレベルで行うことができます (現在はグループに対してのみ)。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-109">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="2fc7d-110">作成要求では、テンプレートで定義されているすべての設定の settingvalues を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-110">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="2fc7d-111">グループ固有の設定では、グループのメンバーがゲストユーザーを招待できるかどうかを制御する設定のみが可能です。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-111">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="2fc7d-112">これは、グループにゲストユーザーを追加する機能が一般に利用可能になったときに、この動作を制御します。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-112">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="2fc7d-113">**注**: この API のベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-113">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="2fc7d-114">この API の/v1.0 バージョンが、 *groupsettings を作成*する名前に変更されました。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-114">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="2fc7d-115">テンプレートと、ベータ版でサポートされているプロパティの一覧については、 [directorysettingtemplate クエリ](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta)を使用してください。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-115">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="2fc7d-116">(v2.0 エンドポイントの場合は、[ [groupsettingtemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)] を呼び出します)。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-116">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="2fc7d-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2fc7d-117">Permissions</span></span>
<span data-ttu-id="2fc7d-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fc7d-120">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2fc7d-120">Permission type</span></span>      | <span data-ttu-id="2fc7d-121">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2fc7d-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fc7d-122">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2fc7d-122">Delegated (work or school account)</span></span> | <span data-ttu-id="2fc7d-123">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2fc7d-123">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2fc7d-124">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2fc7d-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fc7d-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-125">Not supported.</span></span>    |
|<span data-ttu-id="2fc7d-126">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2fc7d-126">Application</span></span> | <span data-ttu-id="2fc7d-127">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fc7d-127">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fc7d-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2fc7d-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="2fc7d-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2fc7d-129">Request headers</span></span>
| <span data-ttu-id="2fc7d-130">名前</span><span class="sxs-lookup"><span data-stu-id="2fc7d-130">Name</span></span>       | <span data-ttu-id="2fc7d-131">説明</span><span class="sxs-lookup"><span data-stu-id="2fc7d-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2fc7d-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fc7d-132">Authorization</span></span>  | <span data-ttu-id="2fc7d-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fc7d-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="2fc7d-135">Request body</span></span>
<span data-ttu-id="2fc7d-136">要求本文で、 [directorysetting](../resources/directorysetting.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-136">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="2fc7d-137">ただし、設定の表示名は、参照される設定テンプレート名に基づいて設定されます。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-137">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="2fc7d-138">応答</span><span class="sxs-lookup"><span data-stu-id="2fc7d-138">Response</span></span>

<span data-ttu-id="2fc7d-139">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[directorysetting](../resources/directorysetting.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-139">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fc7d-140">例</span><span class="sxs-lookup"><span data-stu-id="2fc7d-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fc7d-141">要求</span><span class="sxs-lookup"><span data-stu-id="2fc7d-141">Request</span></span>
<span data-ttu-id="2fc7d-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
Content-type: application/json
Content-length: 222

{
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
<span data-ttu-id="2fc7d-143">要求本文で、 [directorysetting](../resources/directorysetting.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-143">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2fc7d-144">応答</span><span class="sxs-lookup"><span data-stu-id="2fc7d-144">Response</span></span>
<span data-ttu-id="2fc7d-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2fc7d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
    "@odata.context": "https://graph.microsoft.com/stagingbeta/$metadata#settings/$entity",
    "id": "id-value",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-post-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
