---
title: デバイスを更新する
description: デバイスのプロパティを更新します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb6e837a1ce90203558d5e3ca79da8beb6d1b880
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437167"
---
# <a name="update-device"></a><span data-ttu-id="88a00-103">デバイスを更新する</span><span class="sxs-lookup"><span data-stu-id="88a00-103">Update device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88a00-104">デバイスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="88a00-104">Update the properties of a device.</span></span>

<span data-ttu-id="88a00-105">承認済みモバイル デバイス管理 (MDM) アプリによって、デバイスの特定のプロパティのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="88a00-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="88a00-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="88a00-106">Permissions</span></span>
<span data-ttu-id="88a00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88a00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88a00-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="88a00-109">Permission type</span></span>      | <span data-ttu-id="88a00-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="88a00-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88a00-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="88a00-111">Delegated (work or school account)</span></span> | <span data-ttu-id="88a00-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88a00-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="88a00-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="88a00-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88a00-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88a00-114">Not supported.</span></span> |
|<span data-ttu-id="88a00-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="88a00-115">Application</span></span> | <span data-ttu-id="88a00-116">非サポート</span><span class="sxs-lookup"><span data-stu-id="88a00-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="88a00-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88a00-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="88a00-118">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="88a00-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88a00-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88a00-119">Request headers</span></span>
| <span data-ttu-id="88a00-120">名前</span><span class="sxs-lookup"><span data-stu-id="88a00-120">Name</span></span>       | <span data-ttu-id="88a00-121">型</span><span class="sxs-lookup"><span data-stu-id="88a00-121">Type</span></span> | <span data-ttu-id="88a00-122">説明</span><span class="sxs-lookup"><span data-stu-id="88a00-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="88a00-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88a00-123">Authorization</span></span>  | <span data-ttu-id="88a00-124">string</span><span class="sxs-lookup"><span data-stu-id="88a00-124">string</span></span>  | <span data-ttu-id="88a00-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="88a00-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88a00-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="88a00-127">Request body</span></span>

<span data-ttu-id="88a00-128">要求本文で、更新する[デバイス](../resources/device.md) プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="88a00-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="88a00-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="88a00-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="88a00-130">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="88a00-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="88a00-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88a00-131">Property</span></span>     | <span data-ttu-id="88a00-132">型</span><span class="sxs-lookup"><span data-stu-id="88a00-132">Type</span></span>   |<span data-ttu-id="88a00-133">説明</span><span class="sxs-lookup"><span data-stu-id="88a00-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88a00-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="88a00-134">accountEnabled</span></span>|<span data-ttu-id="88a00-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="88a00-135">Boolean</span></span>| <span data-ttu-id="88a00-136">アカウントが有効な場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="88a00-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="88a00-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="88a00-137">operatingSystem</span></span>|<span data-ttu-id="88a00-138">文字列</span><span class="sxs-lookup"><span data-stu-id="88a00-138">String</span></span>|<span data-ttu-id="88a00-139">デバイス上のオペレーティング システムの種類。</span><span class="sxs-lookup"><span data-stu-id="88a00-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="88a00-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="88a00-140">operatingSystemVersion</span></span>|<span data-ttu-id="88a00-141">String</span><span class="sxs-lookup"><span data-stu-id="88a00-141">String</span></span>|<span data-ttu-id="88a00-142">デバイス上のオペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="88a00-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="88a00-143">displayName</span><span class="sxs-lookup"><span data-stu-id="88a00-143">displayName</span></span>|<span data-ttu-id="88a00-144">String</span><span class="sxs-lookup"><span data-stu-id="88a00-144">String</span></span>|<span data-ttu-id="88a00-145">デバイスの表示名。</span><span class="sxs-lookup"><span data-stu-id="88a00-145">The display name for the device.</span></span>|
|<span data-ttu-id="88a00-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="88a00-146">isCompliant</span></span>|<span data-ttu-id="88a00-147">ブール値</span><span class="sxs-lookup"><span data-stu-id="88a00-147">Boolean</span></span>|<span data-ttu-id="88a00-148">デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="88a00-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="88a00-149">これは、任意のデバイスの OS タイプに対して、または Windows OS デバイス用の承認された[MDM アプリ](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)によってのみ、Intune によって更新できます。</span><span class="sxs-lookup"><span data-stu-id="88a00-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="88a00-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="88a00-150">isManaged</span></span>|<span data-ttu-id="88a00-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="88a00-151">Boolean</span></span>|<span data-ttu-id="88a00-152">デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="88a00-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="88a00-153">これは、任意のデバイスの OS タイプに対して、または Windows OS デバイス用の承認された[MDM アプリ](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)によってのみ、Intune によって更新できます。</span><span class="sxs-lookup"><span data-stu-id="88a00-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="88a00-154">**デバイス**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`PATCH` 、操作を使用して、既存の**デバイス**インスタンスの拡張機能のカスタムプロパティで、独自のアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="88a00-154">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="88a00-155">応答</span><span class="sxs-lookup"><span data-stu-id="88a00-155">Response</span></span>

<span data-ttu-id="88a00-156">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="88a00-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="88a00-157">例</span><span class="sxs-lookup"><span data-stu-id="88a00-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="88a00-158">要求</span><span class="sxs-lookup"><span data-stu-id="88a00-158">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="88a00-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="88a00-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/beta/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="88a00-160">C#</span><span class="sxs-lookup"><span data-stu-id="88a00-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88a00-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="88a00-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="88a00-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="88a00-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="88a00-163">応答</span><span class="sxs-lookup"><span data-stu-id="88a00-163">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="88a00-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="88a00-164">See also</span></span>

- [<span data-ttu-id="88a00-165">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="88a00-165">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="88a00-166">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="88a00-166">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="88a00-167">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="88a00-167">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
