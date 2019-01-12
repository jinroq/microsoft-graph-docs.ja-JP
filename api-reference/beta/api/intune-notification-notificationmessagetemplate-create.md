---
title: notificationMessageTemplate の作成
description: 新しい notificationMessageTemplate オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 94b6f1ba814eb426b61e2d7769529e1353326cc4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978565"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="9203b-103">notificationMessageTemplate の作成</span><span class="sxs-lookup"><span data-stu-id="9203b-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="9203b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9203b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9203b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9203b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9203b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9203b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9203b-107">新しい [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9203b-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9203b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9203b-108">Prerequisites</span></span>
<span data-ttu-id="9203b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9203b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9203b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9203b-111">Permission type</span></span>|<span data-ttu-id="9203b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9203b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9203b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9203b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9203b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9203b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9203b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9203b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9203b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9203b-116">Not supported.</span></span>|
|<span data-ttu-id="9203b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9203b-117">Application</span></span>|<span data-ttu-id="9203b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9203b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9203b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9203b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="9203b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9203b-120">Request headers</span></span>
|<span data-ttu-id="9203b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9203b-121">Header</span></span>|<span data-ttu-id="9203b-122">値</span><span class="sxs-lookup"><span data-stu-id="9203b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9203b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9203b-123">Authorization</span></span>|<span data-ttu-id="9203b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9203b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9203b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9203b-125">Accept</span></span>|<span data-ttu-id="9203b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9203b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9203b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9203b-127">Request body</span></span>
<span data-ttu-id="9203b-128">要求の本文で、notificationMessageTemplate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9203b-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="9203b-129">次の表に、notificationMessageTemplate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9203b-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="9203b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9203b-130">Property</span></span>|<span data-ttu-id="9203b-131">型</span><span class="sxs-lookup"><span data-stu-id="9203b-131">Type</span></span>|<span data-ttu-id="9203b-132">説明</span><span class="sxs-lookup"><span data-stu-id="9203b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9203b-133">ID</span><span class="sxs-lookup"><span data-stu-id="9203b-133">id</span></span>|<span data-ttu-id="9203b-134">String</span><span class="sxs-lookup"><span data-stu-id="9203b-134">String</span></span>|<span data-ttu-id="9203b-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9203b-135">Key of the entity.</span></span>|
|<span data-ttu-id="9203b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9203b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9203b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9203b-137">DateTimeOffset</span></span>|<span data-ttu-id="9203b-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9203b-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9203b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="9203b-139">displayName</span></span>|<span data-ttu-id="9203b-140">String</span><span class="sxs-lookup"><span data-stu-id="9203b-140">String</span></span>|<span data-ttu-id="9203b-141">通知メッセージ テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="9203b-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="9203b-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="9203b-142">defaultLocale</span></span>|<span data-ttu-id="9203b-143">String</span><span class="sxs-lookup"><span data-stu-id="9203b-143">String</span></span>|<span data-ttu-id="9203b-144">要求されたロケールが使用できないときにフォールバックする既定のロケール。</span><span class="sxs-lookup"><span data-stu-id="9203b-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="9203b-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="9203b-145">brandingOptions</span></span>|[<span data-ttu-id="9203b-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="9203b-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="9203b-147">メッセージ テンプレートのブランド化オプション。</span><span class="sxs-lookup"><span data-stu-id="9203b-147">The Message Template Branding Options.</span></span> <span data-ttu-id="9203b-148">ブランド化は、Intune 管理コンソールで定義されます。</span><span class="sxs-lookup"><span data-stu-id="9203b-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="9203b-149">可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。</span><span class="sxs-lookup"><span data-stu-id="9203b-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="9203b-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9203b-150">roleScopeTagIds</span></span>|<span data-ttu-id="9203b-151">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9203b-151">String collection</span></span>|<span data-ttu-id="9203b-152">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="9203b-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="9203b-153">応答</span><span class="sxs-lookup"><span data-stu-id="9203b-153">Response</span></span>
<span data-ttu-id="9203b-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9203b-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9203b-155">例</span><span class="sxs-lookup"><span data-stu-id="9203b-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="9203b-156">要求</span><span class="sxs-lookup"><span data-stu-id="9203b-156">Request</span></span>
<span data-ttu-id="9203b-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9203b-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="9203b-158">応答</span><span class="sxs-lookup"><span data-stu-id="9203b-158">Response</span></span>
<span data-ttu-id="9203b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9203b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





