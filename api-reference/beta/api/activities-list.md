---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: ファイルの活動
localization_priority: Normal
ms.openlocfilehash: 55719340eb8baa565c79802403909b66ee5a4e49
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833769"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="9f71f-102">アクティビティを列挙する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="9f71f-102">Enumerate activities (preview)</span></span>

> <span data-ttu-id="9f71f-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f71f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f71f-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f71f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f71f-105">アイテムまたは階層の下で行われた最近の[アクティビティ][]を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9f71f-105">List the recent [activities][] that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="9f71f-106">**メモ:** アクティビティは限定されたプレビューのため、まだすべてのテナントによる利用はできません。</span><span class="sxs-lookup"><span data-stu-id="9f71f-106">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[アクティビティ]: ../resources/itemactivity.md
[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="9f71f-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9f71f-108">Permissions</span></span>

<span data-ttu-id="9f71f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f71f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f71f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f71f-111">Permission type</span></span>                        | <span data-ttu-id="9f71f-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f71f-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="9f71f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f71f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f71f-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f71f-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="9f71f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f71f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f71f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f71f-116">Not supported.</span></span>
|<span data-ttu-id="9f71f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f71f-117">Application</span></span>                            | <span data-ttu-id="9f71f-118">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f71f-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="9f71f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f71f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="9f71f-120">例</span><span class="sxs-lookup"><span data-stu-id="9f71f-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9f71f-121">要求</span><span class="sxs-lookup"><span data-stu-id="9f71f-121">Request</span></span>

<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```

#### <a name="response"></a><span data-ttu-id="9f71f-122">応答</span><span class="sxs-lookup"><span data-stu-id="9f71f-122">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites"
} -->
