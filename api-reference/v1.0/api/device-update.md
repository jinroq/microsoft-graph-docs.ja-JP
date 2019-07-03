---
title: デバイスを更新する
description: 登録済みデバイスのプロパティを更新します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 704c42fb4479408e02853f79669d2e724bdf7f0b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449107"
---
# <a name="update-device"></a><span data-ttu-id="aba82-103">デバイスを更新する</span><span class="sxs-lookup"><span data-stu-id="aba82-103">Update device</span></span>

<span data-ttu-id="aba82-104">登録済みデバイスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aba82-104">Update the properties of a registered device.</span></span>

<span data-ttu-id="aba82-105">承認済みモバイル デバイス管理 (MDM) アプリによって、デバイスの特定のプロパティのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="aba82-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="aba82-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aba82-106">Permissions</span></span>
<span data-ttu-id="aba82-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aba82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aba82-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aba82-109">Permission type</span></span>      | <span data-ttu-id="aba82-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aba82-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aba82-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aba82-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aba82-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aba82-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="aba82-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aba82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aba82-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aba82-114">Not supported.</span></span> |
|<span data-ttu-id="aba82-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aba82-115">Application</span></span> | <span data-ttu-id="aba82-116">非サポート</span><span class="sxs-lookup"><span data-stu-id="aba82-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="aba82-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aba82-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="aba82-118">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="aba82-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aba82-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aba82-119">Request headers</span></span>
| <span data-ttu-id="aba82-120">名前</span><span class="sxs-lookup"><span data-stu-id="aba82-120">Name</span></span>       | <span data-ttu-id="aba82-121">型</span><span class="sxs-lookup"><span data-stu-id="aba82-121">Type</span></span> | <span data-ttu-id="aba82-122">説明</span><span class="sxs-lookup"><span data-stu-id="aba82-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aba82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aba82-123">Authorization</span></span>  | <span data-ttu-id="aba82-124">string</span><span class="sxs-lookup"><span data-stu-id="aba82-124">string</span></span>  | <span data-ttu-id="aba82-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aba82-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aba82-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="aba82-127">Request body</span></span>

<span data-ttu-id="aba82-128">要求本文で、更新する[デバイス](../resources/device.md) プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="aba82-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="aba82-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="aba82-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="aba82-130">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="aba82-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="aba82-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aba82-131">Property</span></span>     | <span data-ttu-id="aba82-132">型</span><span class="sxs-lookup"><span data-stu-id="aba82-132">Type</span></span>   |<span data-ttu-id="aba82-133">説明</span><span class="sxs-lookup"><span data-stu-id="aba82-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aba82-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="aba82-134">accountEnabled</span></span>|<span data-ttu-id="aba82-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="aba82-135">Boolean</span></span>| <span data-ttu-id="aba82-136">アカウントが有効な場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="aba82-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="aba82-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="aba82-137">operatingSystem</span></span>|<span data-ttu-id="aba82-138">文字列</span><span class="sxs-lookup"><span data-stu-id="aba82-138">String</span></span>|<span data-ttu-id="aba82-139">デバイス上のオペレーティング システムの種類。</span><span class="sxs-lookup"><span data-stu-id="aba82-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="aba82-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="aba82-140">operatingSystemVersion</span></span>|<span data-ttu-id="aba82-141">String</span><span class="sxs-lookup"><span data-stu-id="aba82-141">String</span></span>|<span data-ttu-id="aba82-142">デバイス上のオペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="aba82-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="aba82-143">displayName</span><span class="sxs-lookup"><span data-stu-id="aba82-143">displayName</span></span>|<span data-ttu-id="aba82-144">String</span><span class="sxs-lookup"><span data-stu-id="aba82-144">String</span></span>|<span data-ttu-id="aba82-145">デバイスの表示名。</span><span class="sxs-lookup"><span data-stu-id="aba82-145">The display name for the device.</span></span>|
|<span data-ttu-id="aba82-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="aba82-146">isCompliant</span></span>|<span data-ttu-id="aba82-147">ブール値</span><span class="sxs-lookup"><span data-stu-id="aba82-147">Boolean</span></span>|<span data-ttu-id="aba82-148">デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="aba82-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="aba82-149">これは、任意のデバイスの OS タイプに対して、または Windows OS デバイス用の承認された[MDM アプリ](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)によってのみ、Intune によって更新できます。</span><span class="sxs-lookup"><span data-stu-id="aba82-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="aba82-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="aba82-150">isManaged</span></span>|<span data-ttu-id="aba82-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="aba82-151">Boolean</span></span>|<span data-ttu-id="aba82-152">デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="aba82-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="aba82-153">これは、任意のデバイスの OS タイプに対して、または Windows OS デバイス用の承認された[MDM アプリ](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)によってのみ、Intune によって更新できます。</span><span class="sxs-lookup"><span data-stu-id="aba82-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="aba82-154">応答</span><span class="sxs-lookup"><span data-stu-id="aba82-154">Response</span></span>

<span data-ttu-id="aba82-155">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="aba82-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aba82-156">例</span><span class="sxs-lookup"><span data-stu-id="aba82-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aba82-157">要求</span><span class="sxs-lookup"><span data-stu-id="aba82-157">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aba82-158">プロトコル</span><span class="sxs-lookup"><span data-stu-id="aba82-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aba82-159">C#</span><span class="sxs-lookup"><span data-stu-id="aba82-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aba82-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="aba82-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aba82-161">目的-C</span><span class="sxs-lookup"><span data-stu-id="aba82-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aba82-162">応答</span><span class="sxs-lookup"><span data-stu-id="aba82-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
