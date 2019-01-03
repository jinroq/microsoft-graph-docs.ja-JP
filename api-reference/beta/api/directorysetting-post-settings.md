---
title: ディレクトリの設定を作成します。
description: DirectorySettingTemplates で利用可能なテンプレートに基づいて、新しい設定を作成するのにには、この API を使用します。 テナント レベルまたはオブジェクト レベルでこれらの設定ができます (現在のグループに対してのみ)。 テンプレートで定義されているすべての設定の作成の要求に settingValues を入力してください。 グループに固有の設定のみの設定を制御するグループのメンバーは、ゲスト ユーザーを招待できるかどうかを設定できます。 ゲスト ユーザーをグループに追加することが一般的に使用できるとは、この動作が適用されます。
ms.openlocfilehash: 40e90f66c43032deea8ee866b13508fd73c0f17f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068905"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="0663c-107">ディレクトリの設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="0663c-107">Create a directory setting</span></span>

> <span data-ttu-id="0663c-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0663c-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0663c-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0663c-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0663c-110">DirectorySettingTemplates で利用可能なテンプレートに基づいて、新しい設定を作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="0663c-110">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="0663c-111">テナント レベルまたはオブジェクト レベルでこれらの設定ができます (現在のグループに対してのみ)。</span><span class="sxs-lookup"><span data-stu-id="0663c-111">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="0663c-112">テンプレートで定義されているすべての設定の作成の要求に settingValues を入力してください。</span><span class="sxs-lookup"><span data-stu-id="0663c-112">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="0663c-113">グループに固有の設定のみの設定を制御するグループのメンバーは、ゲスト ユーザーを招待できるかどうかを設定できます。</span><span class="sxs-lookup"><span data-stu-id="0663c-113">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="0663c-114">ゲスト ユーザーをグループに追加することが一般的に使用できるとは、この動作が適用されます。</span><span class="sxs-lookup"><span data-stu-id="0663c-114">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="0663c-115">**注**: この API の/beta バージョンは、のみのグループに適用されます。</span><span class="sxs-lookup"><span data-stu-id="0663c-115">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="0663c-116">この API の/v1.0 バージョン*を作成する groupSettings*の名前は。</span><span class="sxs-lookup"><span data-stu-id="0663c-116">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="0663c-117">テンプレートとベータ版でサポートしているプロパティのリストは、 [directorySettingTemplate クエリ](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta)を使用します。</span><span class="sxs-lookup"><span data-stu-id="0663c-117">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="0663c-118">( [GroupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)を呼び出す v1.0 のエンドポイントに対して)。</span><span class="sxs-lookup"><span data-stu-id="0663c-118">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="0663c-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0663c-119">Permissions</span></span>
<span data-ttu-id="0663c-p106">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0663c-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0663c-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0663c-122">Permission type</span></span>      | <span data-ttu-id="0663c-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0663c-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0663c-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0663c-124">Delegated (work or school account)</span></span> | <span data-ttu-id="0663c-125">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0663c-125">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0663c-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0663c-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0663c-127">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0663c-127">Not supported.</span></span>    |
|<span data-ttu-id="0663c-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0663c-128">Application</span></span> | <span data-ttu-id="0663c-129">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0663c-129">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0663c-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0663c-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="0663c-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0663c-131">Request headers</span></span>
| <span data-ttu-id="0663c-132">名前</span><span class="sxs-lookup"><span data-stu-id="0663c-132">Name</span></span>       | <span data-ttu-id="0663c-133">説明</span><span class="sxs-lookup"><span data-stu-id="0663c-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0663c-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="0663c-134">Authorization</span></span>  | <span data-ttu-id="0663c-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0663c-p107">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0663c-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="0663c-137">Request body</span></span>
<span data-ttu-id="0663c-138">要求の本文には、 [directorySetting](../resources/directorysetting.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="0663c-138">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="0663c-139">ただし、設定の表示名が設定に基づいて参照設定テンプレート名を。</span><span class="sxs-lookup"><span data-stu-id="0663c-139">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="0663c-140">応答</span><span class="sxs-lookup"><span data-stu-id="0663c-140">Response</span></span>

<span data-ttu-id="0663c-141">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[directorySetting](../resources/directorysetting.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0663c-141">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0663c-142">例</span><span class="sxs-lookup"><span data-stu-id="0663c-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0663c-143">要求</span><span class="sxs-lookup"><span data-stu-id="0663c-143">Request</span></span>
<span data-ttu-id="0663c-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0663c-144">Here is an example of the request.</span></span>
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
<span data-ttu-id="0663c-145">要求の本文には、 [directorySetting](../resources/directorysetting.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="0663c-145">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0663c-146">応答</span><span class="sxs-lookup"><span data-stu-id="0663c-146">Response</span></span>
<span data-ttu-id="0663c-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0663c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->