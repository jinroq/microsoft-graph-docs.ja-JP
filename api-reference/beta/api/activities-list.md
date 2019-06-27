---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: ファイルアクティビティ
localization_priority: Normal
ms.openlocfilehash: db1edeb786cfaf7d0257b0097b4403c95d281eb2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258780"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="4ec74-102">アクティビティを列挙する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="4ec74-102">Enumerate activities (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ec74-103">アイテムまたは階層の下で行われた最近の[アクティビティ](../resources/itemactivity.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4ec74-103">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="4ec74-104">**メモ:** アクティビティは限定されたプレビューのため、まだすべてのテナントによる利用はできません。</span><span class="sxs-lookup"><span data-stu-id="4ec74-104">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="4ec74-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4ec74-105">Permissions</span></span>

<span data-ttu-id="4ec74-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ec74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ec74-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4ec74-108">Permission type</span></span>                        | <span data-ttu-id="4ec74-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4ec74-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="4ec74-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4ec74-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ec74-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ec74-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="4ec74-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ec74-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ec74-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ec74-113">Not supported.</span></span>
|<span data-ttu-id="4ec74-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4ec74-114">Application</span></span>                            | <span data-ttu-id="4ec74-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ec74-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4ec74-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4ec74-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="4ec74-117">例</span><span class="sxs-lookup"><span data-stu-id="4ec74-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4ec74-118">要求</span><span class="sxs-lookup"><span data-stu-id="4ec74-118">Request</span></span>

<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```

#### <a name="response"></a><span data-ttu-id="4ec74-119">応答</span><span class="sxs-lookup"><span data-stu-id="4ec74-119">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivity)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "action": {
                "comment": {}
            },
            "actor": {
                "user": {
                    "displayName": "Xavier Wilke"
                }
            },
            "id": "EJalEvjV1EgIYFQAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-29T18:34:40Z"
            }
        },
        {
            "action": {
                "edit": {},
                "version": {
                    "newVersion": "2.0"
                }
            },
            "actor": {
                "user": {
                    "displayName": "Judith Clemons"
                }
            },
            "id": "cInT6/fV1EgFYFQAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-29T16:23:35Z"
            }
        },
        {
            "action": {
                "mention": {
                    "mentionees": [
                        {
                            "user": {
                                "displayName": "Judith Clemons"
                            }
                        }
                    ]
                }
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "EBJa0vPV1EjFX1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:14:14Z"
            }
        },
        {
            "action": {
                "rename": {
                    "oldName": "Document2.docx"
                }
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "QFJFlfPV1Ei/X1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:12:32Z"
            }
        },
        {
            "action": {
                "create": {}
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "IJydkPPV1Ei9X1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:02:24Z"
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4ec74-120">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="4ec74-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4ec74-121">C#</span><span class="sxs-lookup"><span data-stu-id="4ec74-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-activities-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4ec74-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="4ec74-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-activities-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4ec74-123">目的-C</span><span class="sxs-lookup"><span data-stu-id="4ec74-123">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list-activities-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
    "Error: /api-reference/beta/api/activities-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/activities-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/activities-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
