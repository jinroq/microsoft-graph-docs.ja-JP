---
title: deviceManagementAbstractComplexSettingInstance を作成する
description: 新しい deviceManagementAbstractComplexSettingInstance オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 78dfa99d046782ed68432268b0c8ad6e58cf8ac8
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522819"
---
# <a name="create-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="baaa4-103">deviceManagementAbstractComplexSettingInstance を作成する</span><span class="sxs-lookup"><span data-stu-id="baaa4-103">Create deviceManagementAbstractComplexSettingInstance</span></span>

> <span data-ttu-id="baaa4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baaa4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baaa4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="baaa4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baaa4-106">新しい[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="baaa4-106">Create a new [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="baaa4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="baaa4-107">Prerequisites</span></span>
<span data-ttu-id="baaa4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="baaa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baaa4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="baaa4-110">Permission type</span></span>|<span data-ttu-id="baaa4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="baaa4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baaa4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="baaa4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="baaa4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baaa4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="baaa4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="baaa4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baaa4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baaa4-115">Not supported.</span></span>|
|<span data-ttu-id="baaa4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="baaa4-116">Application</span></span>|<span data-ttu-id="baaa4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baaa4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="baaa4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="baaa4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/settings
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="baaa4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="baaa4-119">Request headers</span></span>
|<span data-ttu-id="baaa4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="baaa4-120">Header</span></span>|<span data-ttu-id="baaa4-121">値</span><span class="sxs-lookup"><span data-stu-id="baaa4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baaa4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="baaa4-122">Authorization</span></span>|<span data-ttu-id="baaa4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="baaa4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baaa4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="baaa4-124">Accept</span></span>|<span data-ttu-id="baaa4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="baaa4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baaa4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="baaa4-126">Request body</span></span>
<span data-ttu-id="baaa4-127">要求本文で、deviceManagementAbstractComplexSettingInstance オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="baaa4-127">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingInstance object.</span></span>

<span data-ttu-id="baaa4-128">次の表に、deviceManagementAbstractComplexSettingInstance の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="baaa4-128">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingInstance.</span></span>

|<span data-ttu-id="baaa4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="baaa4-129">Property</span></span>|<span data-ttu-id="baaa4-130">型</span><span class="sxs-lookup"><span data-stu-id="baaa4-130">Type</span></span>|<span data-ttu-id="baaa4-131">説明</span><span class="sxs-lookup"><span data-stu-id="baaa4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baaa4-132">id</span><span class="sxs-lookup"><span data-stu-id="baaa4-132">id</span></span>|<span data-ttu-id="baaa4-133">String</span><span class="sxs-lookup"><span data-stu-id="baaa4-133">String</span></span>|<span data-ttu-id="baaa4-134">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="baaa4-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="baaa4-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="baaa4-135">definitionId</span></span>|<span data-ttu-id="baaa4-136">文字列</span><span class="sxs-lookup"><span data-stu-id="baaa4-136">String</span></span>|<span data-ttu-id="baaa4-137">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="baaa4-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="baaa4-138">valuejson</span><span class="sxs-lookup"><span data-stu-id="baaa4-138">valueJson</span></span>|<span data-ttu-id="baaa4-139">文字列</span><span class="sxs-lookup"><span data-stu-id="baaa4-139">String</span></span>|<span data-ttu-id="baaa4-140">[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="baaa4-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="baaa4-141">implementationId</span><span class="sxs-lookup"><span data-stu-id="baaa4-141">implementationId</span></span>|<span data-ttu-id="baaa4-142">文字列</span><span class="sxs-lookup"><span data-stu-id="baaa4-142">String</span></span>|<span data-ttu-id="baaa4-143">この複合設定の選択された実装の定義 ID</span><span class="sxs-lookup"><span data-stu-id="baaa4-143">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="baaa4-144">応答</span><span class="sxs-lookup"><span data-stu-id="baaa4-144">Response</span></span>
<span data-ttu-id="baaa4-145">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="baaa4-145">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baaa4-146">例</span><span class="sxs-lookup"><span data-stu-id="baaa4-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="baaa4-147">要求</span><span class="sxs-lookup"><span data-stu-id="baaa4-147">Request</span></span>
<span data-ttu-id="baaa4-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="baaa4-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```

### <a name="response"></a><span data-ttu-id="baaa4-149">応答</span><span class="sxs-lookup"><span data-stu-id="baaa4-149">Response</span></span>
<span data-ttu-id="baaa4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="baaa4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "id": "433e9565-9565-433e-6595-3e4365953e43",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```







