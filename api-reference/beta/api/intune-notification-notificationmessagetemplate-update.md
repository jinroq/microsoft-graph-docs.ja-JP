---
title: notificationMessageTemplate の更新
description: notificationMessageTemplate オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9db4438ca5b882436fb6454ebb4b80d548a8ef77
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36353170"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="c5e2e-103">notificationMessageTemplate の更新</span><span class="sxs-lookup"><span data-stu-id="c5e2e-103">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="c5e2e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5e2e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5e2e-106">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-106">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5e2e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c5e2e-107">Prerequisites</span></span>
<span data-ttu-id="c5e2e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5e2e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c5e2e-110">Permission type</span></span>|<span data-ttu-id="c5e2e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c5e2e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5e2e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c5e2e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5e2e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5e2e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c5e2e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5e2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5e2e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-115">Not supported.</span></span>|
|<span data-ttu-id="c5e2e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c5e2e-116">Application</span></span>|<span data-ttu-id="c5e2e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5e2e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5e2e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5e2e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="c5e2e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5e2e-119">Request headers</span></span>
|<span data-ttu-id="c5e2e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5e2e-120">Header</span></span>|<span data-ttu-id="c5e2e-121">値</span><span class="sxs-lookup"><span data-stu-id="c5e2e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5e2e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5e2e-122">Authorization</span></span>|<span data-ttu-id="c5e2e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5e2e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c5e2e-124">Accept</span></span>|<span data-ttu-id="c5e2e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5e2e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5e2e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c5e2e-126">Request body</span></span>
<span data-ttu-id="c5e2e-127">要求の本文で、[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-127">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="c5e2e-128">次の表に、[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-128">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="c5e2e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5e2e-129">Property</span></span>|<span data-ttu-id="c5e2e-130">型</span><span class="sxs-lookup"><span data-stu-id="c5e2e-130">Type</span></span>|<span data-ttu-id="c5e2e-131">説明</span><span class="sxs-lookup"><span data-stu-id="c5e2e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5e2e-132">id</span><span class="sxs-lookup"><span data-stu-id="c5e2e-132">id</span></span>|<span data-ttu-id="c5e2e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="c5e2e-133">String</span></span>|<span data-ttu-id="c5e2e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-134">Key of the entity.</span></span>|
|<span data-ttu-id="c5e2e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5e2e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c5e2e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5e2e-136">DateTimeOffset</span></span>|<span data-ttu-id="c5e2e-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c5e2e-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c5e2e-138">displayName</span></span>|<span data-ttu-id="c5e2e-139">String</span><span class="sxs-lookup"><span data-stu-id="c5e2e-139">String</span></span>|<span data-ttu-id="c5e2e-140">通知メッセージ テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="c5e2e-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="c5e2e-141">defaultLocale</span></span>|<span data-ttu-id="c5e2e-142">String</span><span class="sxs-lookup"><span data-stu-id="c5e2e-142">String</span></span>|<span data-ttu-id="c5e2e-143">要求されたロケールが使用できないときにフォールバックする既定のロケール。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="c5e2e-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="c5e2e-144">brandingOptions</span></span>|[<span data-ttu-id="c5e2e-145">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="c5e2e-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="c5e2e-146">メッセージ テンプレートのブランド化オプション。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-146">The Message Template Branding Options.</span></span> <span data-ttu-id="c5e2e-147">ブランド化は、Intune 管理コンソールで定義されます。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="c5e2e-148">可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="c5e2e-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5e2e-149">roleScopeTagIds</span></span>|<span data-ttu-id="c5e2e-150">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="c5e2e-150">String collection</span></span>|<span data-ttu-id="c5e2e-151">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-151">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="c5e2e-152">応答</span><span class="sxs-lookup"><span data-stu-id="c5e2e-152">Response</span></span>
<span data-ttu-id="c5e2e-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-153">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5e2e-154">例</span><span class="sxs-lookup"><span data-stu-id="c5e2e-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5e2e-155">要求</span><span class="sxs-lookup"><span data-stu-id="c5e2e-155">Request</span></span>
<span data-ttu-id="c5e2e-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 259

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="c5e2e-157">応答</span><span class="sxs-lookup"><span data-stu-id="c5e2e-157">Response</span></span>
<span data-ttu-id="c5e2e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c5e2e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```






