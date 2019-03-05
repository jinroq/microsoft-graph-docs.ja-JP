---
title: Create windows10SecureAssessmentConfiguration
description: 新しい windows10SecureAssessmentConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0e8b430023563ddb770b2cf7d4693814f01b4a7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252274"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="1c68f-103">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c68f-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="1c68f-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1c68f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c68f-105">新しい [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1c68f-105">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c68f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1c68f-106">Prerequisites</span></span>
<span data-ttu-id="1c68f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c68f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1c68f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c68f-109">Permission type</span></span>|<span data-ttu-id="1c68f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c68f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c68f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c68f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c68f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c68f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c68f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c68f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c68f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c68f-114">Not supported.</span></span>|
|<span data-ttu-id="1c68f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c68f-115">Application</span></span>|<span data-ttu-id="1c68f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c68f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c68f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c68f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1c68f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c68f-118">Request headers</span></span>
|<span data-ttu-id="1c68f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c68f-119">Header</span></span>|<span data-ttu-id="1c68f-120">値</span><span class="sxs-lookup"><span data-stu-id="1c68f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c68f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c68f-121">Authorization</span></span>|<span data-ttu-id="1c68f-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1c68f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c68f-123">承諾</span><span class="sxs-lookup"><span data-stu-id="1c68f-123">Accept</span></span>|<span data-ttu-id="1c68f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1c68f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c68f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c68f-125">Request body</span></span>
<span data-ttu-id="1c68f-126">要求本文で、windows10SecureAssessmentConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1c68f-126">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="1c68f-127">次の表に、windows10SecureAssessmentConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1c68f-127">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="1c68f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c68f-128">Property</span></span>|<span data-ttu-id="1c68f-129">型</span><span class="sxs-lookup"><span data-stu-id="1c68f-129">Type</span></span>|<span data-ttu-id="1c68f-130">説明</span><span class="sxs-lookup"><span data-stu-id="1c68f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c68f-131">id</span><span class="sxs-lookup"><span data-stu-id="1c68f-131">id</span></span>|<span data-ttu-id="1c68f-132">文字列</span><span class="sxs-lookup"><span data-stu-id="1c68f-132">String</span></span>|<span data-ttu-id="1c68f-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1c68f-133">Key of the entity.</span></span> <span data-ttu-id="1c68f-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c68f-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c68f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c68f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="1c68f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c68f-136">DateTimeOffset</span></span>|<span data-ttu-id="1c68f-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1c68f-137">DateTime the object was last modified.</span></span> <span data-ttu-id="1c68f-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c68f-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c68f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c68f-139">createdDateTime</span></span>|<span data-ttu-id="1c68f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c68f-140">DateTimeOffset</span></span>|<span data-ttu-id="1c68f-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1c68f-141">DateTime the object was created.</span></span> <span data-ttu-id="1c68f-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c68f-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c68f-143">説明</span><span class="sxs-lookup"><span data-stu-id="1c68f-143">description</span></span>|<span data-ttu-id="1c68f-144">文字列</span><span class="sxs-lookup"><span data-stu-id="1c68f-144">String</span></span>|<span data-ttu-id="1c68f-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1c68f-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1c68f-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c68f-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c68f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="1c68f-147">displayName</span></span>|<span data-ttu-id="1c68f-148">String</span><span class="sxs-lookup"><span data-stu-id="1c68f-148">String</span></span>|<span data-ttu-id="1c68f-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1c68f-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1c68f-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c68f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c68f-151">version</span><span class="sxs-lookup"><span data-stu-id="1c68f-151">version</span></span>|<span data-ttu-id="1c68f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1c68f-152">Int32</span></span>|<span data-ttu-id="1c68f-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1c68f-153">Version of the device configuration.</span></span> <span data-ttu-id="1c68f-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1c68f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c68f-155">launchUri</span><span class="sxs-lookup"><span data-stu-id="1c68f-155">launchUri</span></span>|<span data-ttu-id="1c68f-156">String</span><span class="sxs-lookup"><span data-stu-id="1c68f-156">String</span></span>|<span data-ttu-id="1c68f-157">安全性評価ブラウザーを起動すると自動的に読み込まれる評価への URL リンク。</span><span class="sxs-lookup"><span data-stu-id="1c68f-157">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="1c68f-158">有効な URL である必要があります (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="1c68f-158">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="1c68f-159">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="1c68f-159">configurationAccount</span></span>|<span data-ttu-id="1c68f-160">String</span><span class="sxs-lookup"><span data-stu-id="1c68f-160">String</span></span>|<span data-ttu-id="1c68f-161">Windows デバイスにテストを受けさせる際に、それを構成するために使用するアカウント。</span><span class="sxs-lookup"><span data-stu-id="1c68f-161">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="1c68f-162">ユーザーは、ドメイン アカウント (domain\user)、AAD アカウント (username@tenant.com)、ローカル アカウント (username) のいずれでも可能です。</span><span class="sxs-lookup"><span data-stu-id="1c68f-162">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="1c68f-163">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="1c68f-163">allowPrinting</span></span>|<span data-ttu-id="1c68f-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c68f-164">Boolean</span></span>|<span data-ttu-id="1c68f-165">テスト中にアプリが印刷することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c68f-165">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="1c68f-166">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="1c68f-166">allowScreenCapture</span></span>|<span data-ttu-id="1c68f-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c68f-167">Boolean</span></span>|<span data-ttu-id="1c68f-168">テスト中に画面キャプチャ機能を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c68f-168">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="1c68f-169">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="1c68f-169">allowTextSuggestion</span></span>|<span data-ttu-id="1c68f-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c68f-170">Boolean</span></span>|<span data-ttu-id="1c68f-171">テスト中に入力ヒントを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c68f-171">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="1c68f-172">応答</span><span class="sxs-lookup"><span data-stu-id="1c68f-172">Response</span></span>
<span data-ttu-id="1c68f-173">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1c68f-173">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c68f-174">例</span><span class="sxs-lookup"><span data-stu-id="1c68f-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c68f-175">要求</span><span class="sxs-lookup"><span data-stu-id="1c68f-175">Request</span></span>
<span data-ttu-id="1c68f-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1c68f-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="1c68f-177">応答</span><span class="sxs-lookup"><span data-stu-id="1c68f-177">Response</span></span>
<span data-ttu-id="1c68f-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1c68f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```



