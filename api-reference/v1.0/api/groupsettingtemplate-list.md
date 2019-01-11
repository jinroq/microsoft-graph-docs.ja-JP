---
title: groupSettingTemplates のリスト
description: グループ設定テンプレートは、テナント内でグループ設定を作成および使用するための一連のテンプレートを表します。この操作は、使用可能な groupSettingTemplates オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 476577de23bc0fe5c2df9ce37b2d9083105bb6f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869875"
---
# <a name="list-groupsettingtemplates"></a><span data-ttu-id="3d159-104">groupSettingTemplates のリスト</span><span class="sxs-lookup"><span data-stu-id="3d159-104">List groupSettingTemplates</span></span>

<span data-ttu-id="3d159-p102">グループ設定テンプレートは、テナント内でグループ設定を作成および使用するための一連のテンプレートを表します。この操作は、使用可能な groupSettingTemplates オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="3d159-p102">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d159-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3d159-107">Permissions</span></span>

<span data-ttu-id="3d159-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d159-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3d159-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d159-110">Permission type</span></span>      | <span data-ttu-id="3d159-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d159-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d159-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d159-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3d159-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3d159-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3d159-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d159-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d159-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d159-115">Not supported.</span></span>    |
|<span data-ttu-id="3d159-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d159-116">Application</span></span> | <span data-ttu-id="3d159-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d159-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d159-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d159-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3d159-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3d159-119">Optional query parameters</span></span>
<span data-ttu-id="3d159-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3d159-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="3d159-121">**注:** $filter はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d159-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d159-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d159-122">Request headers</span></span>
| <span data-ttu-id="3d159-123">名前</span><span class="sxs-lookup"><span data-stu-id="3d159-123">Name</span></span> | <span data-ttu-id="3d159-124">説明</span><span class="sxs-lookup"><span data-stu-id="3d159-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="3d159-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d159-125">Authorization</span></span>  | <span data-ttu-id="3d159-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3d159-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d159-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d159-128">Request body</span></span>
<span data-ttu-id="3d159-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3d159-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d159-130">応答</span><span class="sxs-lookup"><span data-stu-id="3d159-130">Response</span></span>

<span data-ttu-id="3d159-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupSettingTemplate](../resources/groupsettingtemplate.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3d159-131">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d159-132">例</span><span class="sxs-lookup"><span data-stu-id="3d159-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d159-133">要求</span><span class="sxs-lookup"><span data-stu-id="3d159-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
##### <a name="response"></a><span data-ttu-id="3d159-134">応答</span><span class="sxs-lookup"><span data-stu-id="3d159-134">Response</span></span>

<span data-ttu-id="3d159-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3d159-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
                    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
                    "deletedDateTime": null,
                    "displayName": "Group.Unified",
                    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
                    "values": [
                        {
                            "name": "CustomBlockedWordsList",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "EnableMSStandardBlockedWords",
                            "type": "System.Boolean",
                            "defaultValue": "false",
                            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "ClassificationDescriptions",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
                        }
                    ]
                }
            ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
