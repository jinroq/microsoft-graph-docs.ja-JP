---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: ファイルアクティビティ
localization_priority: Normal
ms.openlocfilehash: 75849fc67febe8c0f22d4dbd057da98aea5e8854
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459492"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="c9c8a-102">アクティビティを列挙する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="c9c8a-102">Enumerate activities (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9c8a-103">アイテムまたは階層の下で行われた最近の[アクティビティ][]を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c9c8a-103">List the recent [activities][] that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="c9c8a-104">**メモ:** アクティビティは限定されたプレビューのため、まだすべてのテナントによる利用はできません。</span><span class="sxs-lookup"><span data-stu-id="c9c8a-104">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[アクティビティ]: ../resources/itemactivity.md
[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="c9c8a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c9c8a-106">Permissions</span></span>

<span data-ttu-id="c9c8a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9c8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9c8a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9c8a-109">Permission type</span></span>                        | <span data-ttu-id="c9c8a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9c8a-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="c9c8a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9c8a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9c8a-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9c8a-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="c9c8a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9c8a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9c8a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9c8a-114">Not supported.</span></span>
|<span data-ttu-id="c9c8a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9c8a-115">Application</span></span>                            | <span data-ttu-id="c9c8a-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9c8a-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c9c8a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9c8a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="c9c8a-118">例</span><span class="sxs-lookup"><span data-stu-id="c9c8a-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c9c8a-119">要求</span><span class="sxs-lookup"><span data-stu-id="c9c8a-119">Request</span></span>

<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```

#### <a name="response"></a><span data-ttu-id="c9c8a-120">応答</span><span class="sxs-lookup"><span data-stu-id="c9c8a-120">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
    "Error: /api-reference/beta/api/activities-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
