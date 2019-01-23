---
title: notificationMessageTemplate の作成
description: 新しい notificationMessageTemplate オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f16d9e679533e56e59393f967b9b192b74f3607b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419822"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="7a076-103">notificationMessageTemplate の作成</span><span class="sxs-lookup"><span data-stu-id="7a076-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="7a076-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7a076-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7a076-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a076-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a076-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7a076-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a076-107">新しい [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7a076-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a076-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7a076-108">Prerequisites</span></span>
<span data-ttu-id="7a076-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a076-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7a076-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7a076-111">Permission type</span></span>|<span data-ttu-id="7a076-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7a076-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a076-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7a076-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a076-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a076-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7a076-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7a076-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a076-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a076-116">Not supported.</span></span>|
|<span data-ttu-id="7a076-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7a076-117">Application</span></span>|<span data-ttu-id="7a076-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a076-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a076-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7a076-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="7a076-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a076-120">Request headers</span></span>
|<span data-ttu-id="7a076-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a076-121">Header</span></span>|<span data-ttu-id="7a076-122">値</span><span class="sxs-lookup"><span data-stu-id="7a076-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a076-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a076-123">Authorization</span></span>|<span data-ttu-id="7a076-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7a076-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a076-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7a076-125">Accept</span></span>|<span data-ttu-id="7a076-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a076-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a076-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7a076-127">Request body</span></span>
<span data-ttu-id="7a076-128">要求の本文で、notificationMessageTemplate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7a076-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="7a076-129">次の表に、notificationMessageTemplate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7a076-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="7a076-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a076-130">Property</span></span>|<span data-ttu-id="7a076-131">型</span><span class="sxs-lookup"><span data-stu-id="7a076-131">Type</span></span>|<span data-ttu-id="7a076-132">説明</span><span class="sxs-lookup"><span data-stu-id="7a076-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a076-133">id</span><span class="sxs-lookup"><span data-stu-id="7a076-133">id</span></span>|<span data-ttu-id="7a076-134">String</span><span class="sxs-lookup"><span data-stu-id="7a076-134">String</span></span>|<span data-ttu-id="7a076-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7a076-135">Key of the entity.</span></span>|
|<span data-ttu-id="7a076-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a076-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7a076-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a076-137">DateTimeOffset</span></span>|<span data-ttu-id="7a076-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7a076-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7a076-139">displayName</span><span class="sxs-lookup"><span data-stu-id="7a076-139">displayName</span></span>|<span data-ttu-id="7a076-140">String</span><span class="sxs-lookup"><span data-stu-id="7a076-140">String</span></span>|<span data-ttu-id="7a076-141">通知メッセージ テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="7a076-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="7a076-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="7a076-142">defaultLocale</span></span>|<span data-ttu-id="7a076-143">String</span><span class="sxs-lookup"><span data-stu-id="7a076-143">String</span></span>|<span data-ttu-id="7a076-144">要求されたロケールが使用できないときにフォールバックする既定のロケール。</span><span class="sxs-lookup"><span data-stu-id="7a076-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="7a076-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="7a076-145">brandingOptions</span></span>|[<span data-ttu-id="7a076-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="7a076-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="7a076-147">メッセージ テンプレートのブランド化オプション。</span><span class="sxs-lookup"><span data-stu-id="7a076-147">The Message Template Branding Options.</span></span> <span data-ttu-id="7a076-148">ブランド化は、Intune 管理コンソールで定義されます。</span><span class="sxs-lookup"><span data-stu-id="7a076-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="7a076-149">可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。</span><span class="sxs-lookup"><span data-stu-id="7a076-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="7a076-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7a076-150">roleScopeTagIds</span></span>|<span data-ttu-id="7a076-151">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7a076-151">String collection</span></span>|<span data-ttu-id="7a076-152">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="7a076-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="7a076-153">応答</span><span class="sxs-lookup"><span data-stu-id="7a076-153">Response</span></span>
<span data-ttu-id="7a076-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7a076-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a076-155">例</span><span class="sxs-lookup"><span data-stu-id="7a076-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a076-156">要求</span><span class="sxs-lookup"><span data-stu-id="7a076-156">Request</span></span>
<span data-ttu-id="7a076-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7a076-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
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

### <a name="response"></a><span data-ttu-id="7a076-158">応答</span><span class="sxs-lookup"><span data-stu-id="7a076-158">Response</span></span>
<span data-ttu-id="7a076-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7a076-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




