---
title: デバイスを更新する
description: デバイスのプロパティを更新します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 70c5e6475f32f7e545371064411885d2690e4f0e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520943"
---
# <a name="update-device"></a><span data-ttu-id="08091-103">デバイスを更新する</span><span class="sxs-lookup"><span data-stu-id="08091-103">Update device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08091-104">デバイスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="08091-104">Update the properties of a device.</span></span>

<span data-ttu-id="08091-105">承認済みモバイル デバイス管理 (MDM) アプリによって、デバイスの特定のプロパティのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="08091-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="08091-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08091-106">Permissions</span></span>
<span data-ttu-id="08091-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08091-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08091-109">Permission type</span></span>      | <span data-ttu-id="08091-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08091-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08091-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08091-111">Delegated (work or school account)</span></span> | <span data-ttu-id="08091-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08091-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="08091-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08091-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08091-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08091-114">Not supported.</span></span> |
|<span data-ttu-id="08091-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08091-115">Application</span></span> | <span data-ttu-id="08091-116">非サポート</span><span class="sxs-lookup"><span data-stu-id="08091-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="08091-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08091-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="08091-118">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="08091-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08091-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08091-119">Request headers</span></span>
| <span data-ttu-id="08091-120">名前</span><span class="sxs-lookup"><span data-stu-id="08091-120">Name</span></span>       | <span data-ttu-id="08091-121">型</span><span class="sxs-lookup"><span data-stu-id="08091-121">Type</span></span> | <span data-ttu-id="08091-122">説明</span><span class="sxs-lookup"><span data-stu-id="08091-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="08091-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08091-123">Authorization</span></span>  | <span data-ttu-id="08091-124">string</span><span class="sxs-lookup"><span data-stu-id="08091-124">string</span></span>  | <span data-ttu-id="08091-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08091-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08091-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="08091-127">Request body</span></span>

<span data-ttu-id="08091-128">要求本文で、更新する[デバイス](../resources/device.md) プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="08091-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="08091-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="08091-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="08091-130">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="08091-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="08091-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08091-131">Property</span></span>     | <span data-ttu-id="08091-132">型</span><span class="sxs-lookup"><span data-stu-id="08091-132">Type</span></span>   |<span data-ttu-id="08091-133">説明</span><span class="sxs-lookup"><span data-stu-id="08091-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08091-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="08091-134">accountEnabled</span></span>|<span data-ttu-id="08091-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="08091-135">Boolean</span></span>| <span data-ttu-id="08091-136">アカウントが有効な場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="08091-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="08091-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="08091-137">operatingSystem</span></span>|<span data-ttu-id="08091-138">String</span><span class="sxs-lookup"><span data-stu-id="08091-138">String</span></span>|<span data-ttu-id="08091-139">デバイス上のオペレーティング システムの種類。</span><span class="sxs-lookup"><span data-stu-id="08091-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="08091-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="08091-140">operatingSystemVersion</span></span>|<span data-ttu-id="08091-141">String</span><span class="sxs-lookup"><span data-stu-id="08091-141">String</span></span>|<span data-ttu-id="08091-142">デバイス上のオペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="08091-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="08091-143">displayName</span><span class="sxs-lookup"><span data-stu-id="08091-143">displayName</span></span>|<span data-ttu-id="08091-144">文字列</span><span class="sxs-lookup"><span data-stu-id="08091-144">String</span></span>|<span data-ttu-id="08091-145">デバイスの表示名。</span><span class="sxs-lookup"><span data-stu-id="08091-145">The display name for the device.</span></span>|
|<span data-ttu-id="08091-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="08091-146">isCompliant</span></span>|<span data-ttu-id="08091-147">ブール値</span><span class="sxs-lookup"><span data-stu-id="08091-147">Boolean</span></span>|<span data-ttu-id="08091-148">デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="08091-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="08091-149">これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。</span><span class="sxs-lookup"><span data-stu-id="08091-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="08091-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="08091-150">isManaged</span></span>|<span data-ttu-id="08091-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="08091-151">Boolean</span></span>|<span data-ttu-id="08091-152">デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="08091-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="08091-153">これはのみ、Intune は、デバイスの OS の種類のか、 [MDM アプリケーションを承認された](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)Windows OS のデバイスで更新できます。</span><span class="sxs-lookup"><span data-stu-id="08091-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="08091-154">使用することができます、**デバイス**・ リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、`PATCH`を追加、更新、または既存の**デバイス**インスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="08091-154">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="08091-155">応答</span><span class="sxs-lookup"><span data-stu-id="08091-155">Response</span></span>

<span data-ttu-id="08091-156">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="08091-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="08091-157">例</span><span class="sxs-lookup"><span data-stu-id="08091-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="08091-158">要求</span><span class="sxs-lookup"><span data-stu-id="08091-158">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="08091-159">応答</span><span class="sxs-lookup"><span data-stu-id="08091-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="08091-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="08091-160">See also</span></span>

- [<span data-ttu-id="08091-161">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="08091-161">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="08091-162">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="08091-162">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- <span data-ttu-id="08091-163">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="08091-163">[Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)</span></span>


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
    "Error: /api-reference/beta/api/device-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
