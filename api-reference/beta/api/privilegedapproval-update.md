---
title: Privilegedapproval の更新
description: Privilegedapproval オブジェクトのプロパティを更新します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6103e01ea9832bd7858215576eaeb4319514d6be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978806"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="cbae7-103">Privilegedapproval の更新</span><span class="sxs-lookup"><span data-stu-id="cbae7-103">Update privilegedapproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbae7-104">Privilegedapproval オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cbae7-104">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cbae7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cbae7-105">Permissions</span></span>
<span data-ttu-id="cbae7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cbae7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cbae7-108">Permission type</span></span>      | <span data-ttu-id="cbae7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cbae7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbae7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cbae7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cbae7-111">PrivilegedAccess、AzureAD、および Directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="cbae7-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cbae7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cbae7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbae7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbae7-113">Not supported.</span></span>    |
|<span data-ttu-id="cbae7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cbae7-114">Application</span></span> | <span data-ttu-id="cbae7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbae7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbae7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cbae7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="cbae7-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbae7-117">Optional request headers</span></span>
| <span data-ttu-id="cbae7-118">名前</span><span class="sxs-lookup"><span data-stu-id="cbae7-118">Name</span></span>       | <span data-ttu-id="cbae7-119">説明</span><span class="sxs-lookup"><span data-stu-id="cbae7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cbae7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbae7-120">Authorization</span></span>  | <span data-ttu-id="cbae7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cbae7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbae7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="cbae7-123">Request body</span></span>
<span data-ttu-id="cbae7-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="cbae7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cbae7-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbae7-127">Property</span></span>     | <span data-ttu-id="cbae7-128">型</span><span class="sxs-lookup"><span data-stu-id="cbae7-128">Type</span></span>   |<span data-ttu-id="cbae7-129">説明</span><span class="sxs-lookup"><span data-stu-id="cbae7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbae7-130">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="cbae7-130">approvalDuration</span></span>|<span data-ttu-id="cbae7-131">期間</span><span class="sxs-lookup"><span data-stu-id="cbae7-131">Duration</span></span>||
|<span data-ttu-id="cbae7-132">approvalState</span><span class="sxs-lookup"><span data-stu-id="cbae7-132">approvalState</span></span>|<span data-ttu-id="cbae7-133">string</span><span class="sxs-lookup"><span data-stu-id="cbae7-133">string</span></span>| <span data-ttu-id="cbae7-134">可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。</span><span class="sxs-lookup"><span data-stu-id="cbae7-134">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="cbae7-135">approvalType</span><span class="sxs-lookup"><span data-stu-id="cbae7-135">approvalType</span></span>|<span data-ttu-id="cbae7-136">String</span><span class="sxs-lookup"><span data-stu-id="cbae7-136">String</span></span>||
|<span data-ttu-id="cbae7-137">approverReason</span><span class="sxs-lookup"><span data-stu-id="cbae7-137">approverReason</span></span>|<span data-ttu-id="cbae7-138">String</span><span class="sxs-lookup"><span data-stu-id="cbae7-138">String</span></span>||
|<span data-ttu-id="cbae7-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="cbae7-139">endDateTime</span></span>|<span data-ttu-id="cbae7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbae7-140">DateTimeOffset</span></span>||
|<span data-ttu-id="cbae7-141">requestorReason</span><span class="sxs-lookup"><span data-stu-id="cbae7-141">requestorReason</span></span>|<span data-ttu-id="cbae7-142">String</span><span class="sxs-lookup"><span data-stu-id="cbae7-142">String</span></span>||
|<span data-ttu-id="cbae7-143">roleId</span><span class="sxs-lookup"><span data-stu-id="cbae7-143">roleId</span></span>|<span data-ttu-id="cbae7-144">String</span><span class="sxs-lookup"><span data-stu-id="cbae7-144">String</span></span>||
|<span data-ttu-id="cbae7-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cbae7-145">startDateTime</span></span>|<span data-ttu-id="cbae7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbae7-146">DateTimeOffset</span></span>||
|<span data-ttu-id="cbae7-147">userId</span><span class="sxs-lookup"><span data-stu-id="cbae7-147">userId</span></span>|<span data-ttu-id="cbae7-148">String</span><span class="sxs-lookup"><span data-stu-id="cbae7-148">String</span></span>||

## <a name="response"></a><span data-ttu-id="cbae7-149">応答</span><span class="sxs-lookup"><span data-stu-id="cbae7-149">Response</span></span>

<span data-ttu-id="cbae7-150">成功した場合、このメソッド`204 No Content`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="cbae7-150">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="cbae7-151">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="cbae7-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="cbae7-152">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="cbae7-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="cbae7-153">例</span><span class="sxs-lookup"><span data-stu-id="cbae7-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbae7-154">要求</span><span class="sxs-lookup"><span data-stu-id="cbae7-154">Request</span></span>
<span data-ttu-id="cbae7-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cbae7-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval{request-id}
Content-type: application/json
Content-length: 180

{
  "approvalState": "approvalState-value",
  "approverReason": "approverReason-value"
}
```
##### <a name="response"></a><span data-ttu-id="cbae7-156">応答</span><span class="sxs-lookup"><span data-stu-id="cbae7-156">Response</span></span>
<span data-ttu-id="cbae7-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cbae7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
