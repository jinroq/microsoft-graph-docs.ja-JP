---
title: Privilegedapproval を更新します。
description: Privilegedapproval オブジェクトのプロパティを更新します。
ms.openlocfilehash: 566351ba89d0173718320640e6fa45b0650aaf0e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067663"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="c0fdc-103">Privilegedapproval を更新します。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-103">Update privilegedapproval</span></span>

> <span data-ttu-id="c0fdc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0fdc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0fdc-106">Privilegedapproval オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-106">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0fdc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c0fdc-107">Permissions</span></span>
<span data-ttu-id="c0fdc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c0fdc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0fdc-110">Permission type</span></span>      | <span data-ttu-id="c0fdc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0fdc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0fdc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0fdc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c0fdc-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0fdc-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0fdc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0fdc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0fdc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-115">Not supported.</span></span>    |
|<span data-ttu-id="c0fdc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0fdc-116">Application</span></span> | <span data-ttu-id="c0fdc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0fdc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0fdc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="c0fdc-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0fdc-119">Optional request headers</span></span>
| <span data-ttu-id="c0fdc-120">名前</span><span class="sxs-lookup"><span data-stu-id="c0fdc-120">Name</span></span>       | <span data-ttu-id="c0fdc-121">説明</span><span class="sxs-lookup"><span data-stu-id="c0fdc-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c0fdc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0fdc-122">Authorization</span></span>  | <span data-ttu-id="c0fdc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0fdc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0fdc-125">Request body</span></span>
<span data-ttu-id="c0fdc-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c0fdc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0fdc-129">Property</span></span>     | <span data-ttu-id="c0fdc-130">型</span><span class="sxs-lookup"><span data-stu-id="c0fdc-130">Type</span></span>   |<span data-ttu-id="c0fdc-131">説明</span><span class="sxs-lookup"><span data-stu-id="c0fdc-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0fdc-132">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="c0fdc-132">approvalDuration</span></span>|<span data-ttu-id="c0fdc-133">Duration</span><span class="sxs-lookup"><span data-stu-id="c0fdc-133">Duration</span></span>||
|<span data-ttu-id="c0fdc-134">approvalState</span><span class="sxs-lookup"><span data-stu-id="c0fdc-134">approvalState</span></span>|<span data-ttu-id="c0fdc-135">文字列</span><span class="sxs-lookup"><span data-stu-id="c0fdc-135">string</span></span>| <span data-ttu-id="c0fdc-136">可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-136">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="c0fdc-137">approvalType</span><span class="sxs-lookup"><span data-stu-id="c0fdc-137">approvalType</span></span>|<span data-ttu-id="c0fdc-138">String</span><span class="sxs-lookup"><span data-stu-id="c0fdc-138">String</span></span>||
|<span data-ttu-id="c0fdc-139">approverReason</span><span class="sxs-lookup"><span data-stu-id="c0fdc-139">approverReason</span></span>|<span data-ttu-id="c0fdc-140">String</span><span class="sxs-lookup"><span data-stu-id="c0fdc-140">String</span></span>||
|<span data-ttu-id="c0fdc-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c0fdc-141">endDateTime</span></span>|<span data-ttu-id="c0fdc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0fdc-142">DateTimeOffset</span></span>||
|<span data-ttu-id="c0fdc-143">requestorReason</span><span class="sxs-lookup"><span data-stu-id="c0fdc-143">requestorReason</span></span>|<span data-ttu-id="c0fdc-144">String</span><span class="sxs-lookup"><span data-stu-id="c0fdc-144">String</span></span>||
|<span data-ttu-id="c0fdc-145">roleId</span><span class="sxs-lookup"><span data-stu-id="c0fdc-145">roleId</span></span>|<span data-ttu-id="c0fdc-146">String</span><span class="sxs-lookup"><span data-stu-id="c0fdc-146">String</span></span>||
|<span data-ttu-id="c0fdc-147">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c0fdc-147">startDateTime</span></span>|<span data-ttu-id="c0fdc-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0fdc-148">DateTimeOffset</span></span>||
|<span data-ttu-id="c0fdc-149">userId</span><span class="sxs-lookup"><span data-stu-id="c0fdc-149">userId</span></span>|<span data-ttu-id="c0fdc-150">String</span><span class="sxs-lookup"><span data-stu-id="c0fdc-150">String</span></span>||

## <a name="response"></a><span data-ttu-id="c0fdc-151">応答</span><span class="sxs-lookup"><span data-stu-id="c0fdc-151">Response</span></span>

<span data-ttu-id="c0fdc-152">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[privilegedApproval](../resources/privilegedapproval.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-152">If successful, this method returns a `200 OK` response code and updated [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="c0fdc-153">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-153">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c0fdc-154">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-154">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="c0fdc-155">例</span><span class="sxs-lookup"><span data-stu-id="c0fdc-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0fdc-156">要求</span><span class="sxs-lookup"><span data-stu-id="c0fdc-156">Request</span></span>
<span data-ttu-id="c0fdc-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval/<id>
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
##### <a name="response"></a><span data-ttu-id="c0fdc-158">応答</span><span class="sxs-lookup"><span data-stu-id="c0fdc-158">Response</span></span>
<span data-ttu-id="c0fdc-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0fdc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
