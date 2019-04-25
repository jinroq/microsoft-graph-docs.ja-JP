---
title: アクセス許可
description: '指定したユーザーが所有している最近削除されたアイテムのリストを取得します。  '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1d57bbada024bdb2358c39ce9183004ea53289dc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555088"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="77493-103">**ユーザーが所有する削除済みアイテムを一覧表示する**</span><span class="sxs-lookup"><span data-stu-id="77493-103">**List deleted items owned by a user**</span></span>

<span data-ttu-id="77493-104">指定したユーザーが所有している最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="77493-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="77493-105">現時点では、削除済みアイテムのリスト機能は、ユーザーが所有する[グループ](../resources/group.md)リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="77493-105">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="77493-106">これは、サービスのアクションであり、改ページ処理をサポートしていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="77493-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="77493-107">API は、ユーザーが所有する最大1000の削除済みオブジェクトを ID で並べ替えて返します。</span><span class="sxs-lookup"><span data-stu-id="77493-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="77493-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="77493-108">Permissions</span></span>

<span data-ttu-id="77493-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77493-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="77493-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77493-111">Permission type</span></span> | <span data-ttu-id="77493-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="77493-112">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="77493-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77493-113">Delegated (work or school account)</span></span> | <span data-ttu-id="77493-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77493-114">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="77493-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77493-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="77493-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77493-116">Not supported.</span></span> |
| <span data-ttu-id="77493-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77493-117">Application</span></span> | <span data-ttu-id="77493-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77493-118">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="77493-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77493-119">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="77493-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77493-120">Request headers</span></span>

| <span data-ttu-id="77493-121">名前</span><span class="sxs-lookup"><span data-stu-id="77493-121">Name</span></span>          | <span data-ttu-id="77493-122">説明</span><span class="sxs-lookup"><span data-stu-id="77493-122">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="77493-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77493-123">Authorization</span></span> | <span data-ttu-id="77493-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="77493-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77493-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="77493-126">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="77493-127">要求本文には、次のパラメーターが必要です。</span><span class="sxs-lookup"><span data-stu-id="77493-127">The request body requires the following parameters:</span></span>

| <span data-ttu-id="77493-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="77493-128">Parameter</span></span>    | <span data-ttu-id="77493-129">型</span><span class="sxs-lookup"><span data-stu-id="77493-129">Type</span></span> |<span data-ttu-id="77493-130">説明</span><span class="sxs-lookup"><span data-stu-id="77493-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77493-131">userId</span><span class="sxs-lookup"><span data-stu-id="77493-131">userId</span></span>|<span data-ttu-id="77493-132">String</span><span class="sxs-lookup"><span data-stu-id="77493-132">String</span></span>|<span data-ttu-id="77493-133">所有者の ID。</span><span class="sxs-lookup"><span data-stu-id="77493-133">ID of the owner.</span></span>|
|<span data-ttu-id="77493-134">type</span><span class="sxs-lookup"><span data-stu-id="77493-134">type</span></span>|<span data-ttu-id="77493-135">String</span><span class="sxs-lookup"><span data-stu-id="77493-135">String</span></span>|<span data-ttu-id="77493-136">取得する、所有されているオブジェクトの種類。`Group`は現在、サポートされている唯一の値です。</span><span class="sxs-lookup"><span data-stu-id="77493-136">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="77493-137">応答</span><span class="sxs-lookup"><span data-stu-id="77493-137">Response</span></span>

<span data-ttu-id="77493-138">成功した`200 OK`要求は応答コードを返します。response オブジェクトには、[ディレクトリ (削除済みアイテム)](../resources/directory.md)のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="77493-138">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="77493-139">例</span><span class="sxs-lookup"><span data-stu-id="77493-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="77493-140">要求</span><span class="sxs-lookup"><span data-stu-id="77493-140">Request</span></span>

<span data-ttu-id="77493-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77493-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="77493-142">応答</span><span class="sxs-lookup"><span data-stu-id="77493-142">Response</span></span>

<span data-ttu-id="77493-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="77493-143">Here is an example of the response.</span></span> <span data-ttu-id="77493-144">注: この応答オブジェクトは、簡潔にするために切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="77493-144">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="77493-145">サポートされているすべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="77493-145">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


