---
title: privilegedapproval の更新
description: privilegedapproval オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: cb108ca35b07138f84a9fd969bfe7c7241e9672e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538678"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="36382-103">privilegedapproval の更新</span><span class="sxs-lookup"><span data-stu-id="36382-103">Update privilegedapproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36382-104">privilegedapproval オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="36382-104">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="36382-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="36382-105">Permissions</span></span>
<span data-ttu-id="36382-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36382-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="36382-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36382-108">Permission type</span></span>      | <span data-ttu-id="36382-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="36382-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36382-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36382-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36382-111">PrivilegedAccess、AzureAD、および directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="36382-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="36382-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36382-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36382-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36382-113">Not supported.</span></span>    |
|<span data-ttu-id="36382-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36382-114">Application</span></span> | <span data-ttu-id="36382-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36382-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36382-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36382-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="36382-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36382-117">Optional request headers</span></span>
| <span data-ttu-id="36382-118">名前</span><span class="sxs-lookup"><span data-stu-id="36382-118">Name</span></span>       | <span data-ttu-id="36382-119">説明</span><span class="sxs-lookup"><span data-stu-id="36382-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="36382-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="36382-120">Authorization</span></span>  | <span data-ttu-id="36382-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="36382-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36382-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="36382-123">Request body</span></span>
<span data-ttu-id="36382-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="36382-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="36382-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36382-127">Property</span></span>     | <span data-ttu-id="36382-128">型</span><span class="sxs-lookup"><span data-stu-id="36382-128">Type</span></span>   |<span data-ttu-id="36382-129">説明</span><span class="sxs-lookup"><span data-stu-id="36382-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36382-130">approvalduration</span><span class="sxs-lookup"><span data-stu-id="36382-130">approvalDuration</span></span>|<span data-ttu-id="36382-131">期間</span><span class="sxs-lookup"><span data-stu-id="36382-131">Duration</span></span>||
|<span data-ttu-id="36382-132">approvalstate</span><span class="sxs-lookup"><span data-stu-id="36382-132">approvalState</span></span>|<span data-ttu-id="36382-133">string</span><span class="sxs-lookup"><span data-stu-id="36382-133">string</span></span>| <span data-ttu-id="36382-134">可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。</span><span class="sxs-lookup"><span data-stu-id="36382-134">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="36382-135">approvalType</span><span class="sxs-lookup"><span data-stu-id="36382-135">approvalType</span></span>|<span data-ttu-id="36382-136">String</span><span class="sxs-lookup"><span data-stu-id="36382-136">String</span></span>||
|<span data-ttu-id="36382-137">approverreason</span><span class="sxs-lookup"><span data-stu-id="36382-137">approverReason</span></span>|<span data-ttu-id="36382-138">String</span><span class="sxs-lookup"><span data-stu-id="36382-138">String</span></span>||
|<span data-ttu-id="36382-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="36382-139">endDateTime</span></span>|<span data-ttu-id="36382-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36382-140">DateTimeOffset</span></span>||
|<span data-ttu-id="36382-141">requestorReason</span><span class="sxs-lookup"><span data-stu-id="36382-141">requestorReason</span></span>|<span data-ttu-id="36382-142">String</span><span class="sxs-lookup"><span data-stu-id="36382-142">String</span></span>||
|<span data-ttu-id="36382-143">roleId</span><span class="sxs-lookup"><span data-stu-id="36382-143">roleId</span></span>|<span data-ttu-id="36382-144">String</span><span class="sxs-lookup"><span data-stu-id="36382-144">String</span></span>||
|<span data-ttu-id="36382-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="36382-145">startDateTime</span></span>|<span data-ttu-id="36382-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36382-146">DateTimeOffset</span></span>||
|<span data-ttu-id="36382-147">userId</span><span class="sxs-lookup"><span data-stu-id="36382-147">userId</span></span>|<span data-ttu-id="36382-148">String</span><span class="sxs-lookup"><span data-stu-id="36382-148">String</span></span>||

## <a name="response"></a><span data-ttu-id="36382-149">応答</span><span class="sxs-lookup"><span data-stu-id="36382-149">Response</span></span>

<span data-ttu-id="36382-150">成功した場合、このメソッド`204 No Content`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="36382-150">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="36382-151">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="36382-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="36382-152">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="36382-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="36382-153">例</span><span class="sxs-lookup"><span data-stu-id="36382-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36382-154">要求</span><span class="sxs-lookup"><span data-stu-id="36382-154">Request</span></span>
<span data-ttu-id="36382-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36382-155">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="36382-156">応答</span><span class="sxs-lookup"><span data-stu-id="36382-156">Response</span></span>
<span data-ttu-id="36382-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36382-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
