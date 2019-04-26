---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: ファイルアクティビティ
localization_priority: Normal
ms.openlocfilehash: 9131146bc627f1f611e817d66dcb86a084fef26f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323021"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="9f6c7-102">アクティビティを列挙する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="9f6c7-102">Enumerate activities (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f6c7-103">アイテムまたは階層の下で行われた最近の[アクティビティ](../resources/itemactivity.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9f6c7-103">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="9f6c7-104">**メモ:** アクティビティは限定されたプレビューのため、まだすべてのテナントによる利用はできません。</span><span class="sxs-lookup"><span data-stu-id="9f6c7-104">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="9f6c7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9f6c7-105">Permissions</span></span>

<span data-ttu-id="9f6c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f6c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f6c7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f6c7-108">Permission type</span></span>                        | <span data-ttu-id="9f6c7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f6c7-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="9f6c7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f6c7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f6c7-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f6c7-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="9f6c7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f6c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f6c7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f6c7-113">Not supported.</span></span>
|<span data-ttu-id="9f6c7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f6c7-114">Application</span></span>                            | <span data-ttu-id="9f6c7-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f6c7-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="9f6c7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f6c7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="9f6c7-117">例</span><span class="sxs-lookup"><span data-stu-id="9f6c7-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9f6c7-118">要求</span><span class="sxs-lookup"><span data-stu-id="9f6c7-118">Request</span></span>

<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```

#### <a name="response"></a><span data-ttu-id="9f6c7-119">応答</span><span class="sxs-lookup"><span data-stu-id="9f6c7-119">Response</span></span>

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
  "suppressions": []
}
-->
