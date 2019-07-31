---
title: メンバーを追加する
description: この API を使用して、管理単位にメンバー (ユーザーまたはグループ) を追加します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6c0465488949244a66c2e25149b4e9958c6b94bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945754"
---
# <a name="add-a-member"></a><span data-ttu-id="f51e1-103">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="f51e1-103">Add a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f51e1-104">この API を使用して、管理単位にメンバー (ユーザーまたはグループ) を追加します。</span><span class="sxs-lookup"><span data-stu-id="f51e1-104">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="f51e1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f51e1-105">Permissions</span></span>
<span data-ttu-id="f51e1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f51e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f51e1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f51e1-108">Permission type</span></span>      | <span data-ttu-id="f51e1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f51e1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f51e1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f51e1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f51e1-111">AdministrativeUnit。すべての Directory.accessasuser.all について</span><span class="sxs-lookup"><span data-stu-id="f51e1-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f51e1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f51e1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f51e1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f51e1-113">Not supported.</span></span>    |
|<span data-ttu-id="f51e1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f51e1-114">Application</span></span> | <span data-ttu-id="f51e1-115">AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="f51e1-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f51e1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f51e1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f51e1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f51e1-117">Request headers</span></span>
| <span data-ttu-id="f51e1-118">名前</span><span class="sxs-lookup"><span data-stu-id="f51e1-118">Name</span></span>      |<span data-ttu-id="f51e1-119">説明</span><span class="sxs-lookup"><span data-stu-id="f51e1-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f51e1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f51e1-120">Authorization</span></span>  | <span data-ttu-id="f51e1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f51e1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f51e1-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f51e1-123">Request body</span></span>
<span data-ttu-id="f51e1-124">要求本文で、追加する[ユーザー](../resources/user.md)、[グループ](../resources/group.md)、または[directoryobject](../resources/directoryobject.md)の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f51e1-124">In the request body, supply a JSON representation of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="f51e1-125">応答</span><span class="sxs-lookup"><span data-stu-id="f51e1-125">Response</span></span>

<span data-ttu-id="f51e1-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f51e1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f51e1-128">例</span><span class="sxs-lookup"><span data-stu-id="f51e1-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f51e1-129">要求</span><span class="sxs-lookup"><span data-stu-id="f51e1-129">Request</span></span>
<span data-ttu-id="f51e1-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f51e1-130">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="f51e1-131">要求本文で、追加する[ユーザー](../resources/user.md)または[グループ](../resources/group.md)オブジェクト`id`の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f51e1-131">In the request body, supply a JSON representation of the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="f51e1-132">応答</span><span class="sxs-lookup"><span data-stu-id="f51e1-132">Response</span></span>
<span data-ttu-id="f51e1-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f51e1-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
