---
title: notificationMessageTemplate の更新
description: notificationMessageTemplate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 484e719b089157ddf18a165b50230ed84c644b2f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974767"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="f3825-103">notificationMessageTemplate の更新</span><span class="sxs-lookup"><span data-stu-id="f3825-103">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="f3825-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3825-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3825-105">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f3825-105">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3825-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3825-106">Prerequisites</span></span>
<span data-ttu-id="f3825-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3825-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3825-109">Permission type</span></span>|<span data-ttu-id="f3825-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3825-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3825-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3825-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3825-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3825-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f3825-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3825-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3825-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3825-114">Not supported.</span></span>|
|<span data-ttu-id="f3825-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3825-115">Application</span></span>|<span data-ttu-id="f3825-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3825-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3825-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3825-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="f3825-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3825-118">Request headers</span></span>
|<span data-ttu-id="f3825-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3825-119">Header</span></span>|<span data-ttu-id="f3825-120">値</span><span class="sxs-lookup"><span data-stu-id="f3825-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3825-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3825-121">Authorization</span></span>|<span data-ttu-id="f3825-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3825-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3825-123">承諾</span><span class="sxs-lookup"><span data-stu-id="f3825-123">Accept</span></span>|<span data-ttu-id="f3825-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3825-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3825-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3825-125">Request body</span></span>
<span data-ttu-id="f3825-126">要求の本文で、[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3825-126">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="f3825-127">次の表に、[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f3825-127">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="f3825-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3825-128">Property</span></span>|<span data-ttu-id="f3825-129">型</span><span class="sxs-lookup"><span data-stu-id="f3825-129">Type</span></span>|<span data-ttu-id="f3825-130">説明</span><span class="sxs-lookup"><span data-stu-id="f3825-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3825-131">id</span><span class="sxs-lookup"><span data-stu-id="f3825-131">id</span></span>|<span data-ttu-id="f3825-132">文字列</span><span class="sxs-lookup"><span data-stu-id="f3825-132">String</span></span>|<span data-ttu-id="f3825-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f3825-133">Key of the entity.</span></span>|
|<span data-ttu-id="f3825-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3825-134">lastModifiedDateTime</span></span>|<span data-ttu-id="f3825-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3825-135">DateTimeOffset</span></span>|<span data-ttu-id="f3825-136">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f3825-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="f3825-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f3825-137">displayName</span></span>|<span data-ttu-id="f3825-138">String</span><span class="sxs-lookup"><span data-stu-id="f3825-138">String</span></span>|<span data-ttu-id="f3825-139">通知メッセージ テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="f3825-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="f3825-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="f3825-140">defaultLocale</span></span>|<span data-ttu-id="f3825-141">String</span><span class="sxs-lookup"><span data-stu-id="f3825-141">String</span></span>|<span data-ttu-id="f3825-142">要求されたロケールが使用できないときにフォールバックする既定のロケール。</span><span class="sxs-lookup"><span data-stu-id="f3825-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="f3825-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="f3825-143">brandingOptions</span></span>|[<span data-ttu-id="f3825-144">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="f3825-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="f3825-145">メッセージ テンプレートのブランド化オプション。</span><span class="sxs-lookup"><span data-stu-id="f3825-145">The Message Template Branding Options.</span></span> <span data-ttu-id="f3825-146">ブランド化は、Intune 管理コンソールで定義されます。</span><span class="sxs-lookup"><span data-stu-id="f3825-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="f3825-147">可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。</span><span class="sxs-lookup"><span data-stu-id="f3825-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="f3825-148">応答</span><span class="sxs-lookup"><span data-stu-id="f3825-148">Response</span></span>
<span data-ttu-id="f3825-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3825-149">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3825-150">例</span><span class="sxs-lookup"><span data-stu-id="f3825-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3825-151">要求</span><span class="sxs-lookup"><span data-stu-id="f3825-151">Request</span></span>
<span data-ttu-id="f3825-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3825-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="f3825-153">応答</span><span class="sxs-lookup"><span data-stu-id="f3825-153">Response</span></span>
<span data-ttu-id="f3825-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3825-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```



