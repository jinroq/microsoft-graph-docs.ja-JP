---
title: SecurityBaselineTemplate を作成する
description: 新しい securityBaselineTemplate オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed38087604f1a6a2e0a5db3321386303fb2b37a4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959461"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="24280-103">SecurityBaselineTemplate を作成する</span><span class="sxs-lookup"><span data-stu-id="24280-103">Create securityBaselineTemplate</span></span>

> <span data-ttu-id="24280-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24280-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24280-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="24280-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24280-106">新しい[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="24280-106">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24280-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="24280-107">Prerequisites</span></span>
<span data-ttu-id="24280-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24280-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24280-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24280-110">Permission type</span></span>|<span data-ttu-id="24280-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="24280-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24280-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24280-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24280-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24280-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24280-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24280-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24280-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24280-115">Not supported.</span></span>|
|<span data-ttu-id="24280-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24280-116">Application</span></span>|<span data-ttu-id="24280-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24280-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24280-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24280-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="24280-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24280-119">Request headers</span></span>
|<span data-ttu-id="24280-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24280-120">Header</span></span>|<span data-ttu-id="24280-121">値</span><span class="sxs-lookup"><span data-stu-id="24280-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24280-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24280-122">Authorization</span></span>|<span data-ttu-id="24280-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="24280-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24280-124">承諾</span><span class="sxs-lookup"><span data-stu-id="24280-124">Accept</span></span>|<span data-ttu-id="24280-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24280-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24280-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="24280-126">Request body</span></span>
<span data-ttu-id="24280-127">要求本文で、securityBaselineTemplate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="24280-127">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="24280-128">次の表に、securityBaselineTemplate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="24280-128">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="24280-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24280-129">Property</span></span>|<span data-ttu-id="24280-130">型</span><span class="sxs-lookup"><span data-stu-id="24280-130">Type</span></span>|<span data-ttu-id="24280-131">説明</span><span class="sxs-lookup"><span data-stu-id="24280-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24280-132">id</span><span class="sxs-lookup"><span data-stu-id="24280-132">id</span></span>|<span data-ttu-id="24280-133">文字列</span><span class="sxs-lookup"><span data-stu-id="24280-133">String</span></span>|<span data-ttu-id="24280-134">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレート ID</span><span class="sxs-lookup"><span data-stu-id="24280-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="24280-135">displayName</span><span class="sxs-lookup"><span data-stu-id="24280-135">displayName</span></span>|<span data-ttu-id="24280-136">String</span><span class="sxs-lookup"><span data-stu-id="24280-136">String</span></span>|<span data-ttu-id="24280-137">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレートの表示名</span><span class="sxs-lookup"><span data-stu-id="24280-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="24280-138">description</span><span class="sxs-lookup"><span data-stu-id="24280-138">description</span></span>|<span data-ttu-id="24280-139">String</span><span class="sxs-lookup"><span data-stu-id="24280-139">String</span></span>|<span data-ttu-id="24280-140">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されるテンプレートの説明</span><span class="sxs-lookup"><span data-stu-id="24280-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="24280-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="24280-141">versionInfo</span></span>|<span data-ttu-id="24280-142">String</span><span class="sxs-lookup"><span data-stu-id="24280-142">String</span></span>|<span data-ttu-id="24280-143">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレートのバージョン情報</span><span class="sxs-lookup"><span data-stu-id="24280-143">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="24280-144">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="24280-144">isDeprecated</span></span>|<span data-ttu-id="24280-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="24280-145">Boolean</span></span>|<span data-ttu-id="24280-146">テンプレートが非推奨になっているか、使用されていません。</span><span class="sxs-lookup"><span data-stu-id="24280-146">The template is deprecated or not.</span></span> <span data-ttu-id="24280-147">推奨されていないテンプレートからは、インテントを作成できません。</span><span class="sxs-lookup"><span data-stu-id="24280-147">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="24280-148">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="24280-148">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="24280-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="24280-149">intentCount</span></span>|<span data-ttu-id="24280-150">Int32</span><span class="sxs-lookup"><span data-stu-id="24280-150">Int32</span></span>|<span data-ttu-id="24280-151">このテンプレートから作成されたインテントの数。</span><span class="sxs-lookup"><span data-stu-id="24280-151">Number of Intents created from this template.</span></span> <span data-ttu-id="24280-152">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="24280-152">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="24280-153">templateType</span><span class="sxs-lookup"><span data-stu-id="24280-153">templateType</span></span>|[<span data-ttu-id="24280-154">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="24280-154">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="24280-155">テンプレートの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="24280-155">The template's type.</span></span> <span data-ttu-id="24280-156">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="24280-156">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="24280-157">可能な値は、`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom` です。</span><span class="sxs-lookup"><span data-stu-id="24280-157">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span></span>|
|<span data-ttu-id="24280-158">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="24280-158">publishedDateTime</span></span>|<span data-ttu-id="24280-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24280-159">DateTimeOffset</span></span>|<span data-ttu-id="24280-160">テンプレートが公開された場合 ( [Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承)</span><span class="sxs-lookup"><span data-stu-id="24280-160">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="24280-161">応答</span><span class="sxs-lookup"><span data-stu-id="24280-161">Response</span></span>
<span data-ttu-id="24280-162">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="24280-162">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24280-163">例</span><span class="sxs-lookup"><span data-stu-id="24280-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="24280-164">要求</span><span class="sxs-lookup"><span data-stu-id="24280-164">Request</span></span>
<span data-ttu-id="24280-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24280-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="24280-166">応答</span><span class="sxs-lookup"><span data-stu-id="24280-166">Response</span></span>
<span data-ttu-id="24280-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24280-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```





