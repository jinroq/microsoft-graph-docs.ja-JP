---
title: securityBaselineSettingState の更新
description: securityBaselineSettingState オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3295cb35fbc9002f458a60d6f1b78a2ef380126b
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524583"
---
# <a name="update-securitybaselinesettingstate"></a><span data-ttu-id="858c8-103">securityBaselineSettingState の更新</span><span class="sxs-lookup"><span data-stu-id="858c8-103">Update securityBaselineSettingState</span></span>

> <span data-ttu-id="858c8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="858c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="858c8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="858c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="858c8-106">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="858c8-106">Update the properties of a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="858c8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="858c8-107">Prerequisites</span></span>
<span data-ttu-id="858c8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="858c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="858c8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="858c8-110">Permission type</span></span>|<span data-ttu-id="858c8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="858c8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="858c8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="858c8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="858c8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="858c8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="858c8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="858c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="858c8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="858c8-115">Not supported.</span></span>|
|<span data-ttu-id="858c8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="858c8-116">Application</span></span>|<span data-ttu-id="858c8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="858c8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="858c8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="858c8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="858c8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="858c8-119">Request headers</span></span>
|<span data-ttu-id="858c8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="858c8-120">Header</span></span>|<span data-ttu-id="858c8-121">値</span><span class="sxs-lookup"><span data-stu-id="858c8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="858c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="858c8-122">Authorization</span></span>|<span data-ttu-id="858c8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="858c8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="858c8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="858c8-124">Accept</span></span>|<span data-ttu-id="858c8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="858c8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="858c8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="858c8-126">Request body</span></span>
<span data-ttu-id="858c8-127">要求本文で、 [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="858c8-127">In the request body, supply a JSON representation for the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

<span data-ttu-id="858c8-128">次の表に、 [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="858c8-128">The following table shows the properties that are required when you create the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>

|<span data-ttu-id="858c8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="858c8-129">Property</span></span>|<span data-ttu-id="858c8-130">型</span><span class="sxs-lookup"><span data-stu-id="858c8-130">Type</span></span>|<span data-ttu-id="858c8-131">説明</span><span class="sxs-lookup"><span data-stu-id="858c8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="858c8-132">id</span><span class="sxs-lookup"><span data-stu-id="858c8-132">id</span></span>|<span data-ttu-id="858c8-133">String</span><span class="sxs-lookup"><span data-stu-id="858c8-133">String</span></span>|<span data-ttu-id="858c8-134">エンティティの一意識別子</span><span class="sxs-lookup"><span data-stu-id="858c8-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="858c8-135">settingName</span><span class="sxs-lookup"><span data-stu-id="858c8-135">settingName</span></span>|<span data-ttu-id="858c8-136">String</span><span class="sxs-lookup"><span data-stu-id="858c8-136">String</span></span>|<span data-ttu-id="858c8-137">レポートされている設定の名前</span><span class="sxs-lookup"><span data-stu-id="858c8-137">The setting name that is being reported</span></span>|
|<span data-ttu-id="858c8-138">state</span><span class="sxs-lookup"><span data-stu-id="858c8-138">state</span></span>|[<span data-ttu-id="858c8-139">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="858c8-139">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="858c8-140">セキュリティベースライン設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="858c8-140">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="858c8-141">可能な値は `unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="858c8-141">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="858c8-142">settingcategoryid</span><span class="sxs-lookup"><span data-stu-id="858c8-142">settingCategoryId</span></span>|<span data-ttu-id="858c8-143">文字列</span><span class="sxs-lookup"><span data-stu-id="858c8-143">String</span></span>|<span data-ttu-id="858c8-144">この設定が属する設定カテゴリ id</span><span class="sxs-lookup"><span data-stu-id="858c8-144">The setting category id which this setting belongs to</span></span>|



## <a name="response"></a><span data-ttu-id="858c8-145">応答</span><span class="sxs-lookup"><span data-stu-id="858c8-145">Response</span></span>
<span data-ttu-id="858c8-146">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="858c8-146">If successful, this method returns a `200 OK` response code and an updated [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="858c8-147">例</span><span class="sxs-lookup"><span data-stu-id="858c8-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="858c8-148">要求</span><span class="sxs-lookup"><span data-stu-id="858c8-148">Request</span></span>
<span data-ttu-id="858c8-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="858c8-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```

### <a name="response"></a><span data-ttu-id="858c8-150">応答</span><span class="sxs-lookup"><span data-stu-id="858c8-150">Response</span></span>
<span data-ttu-id="858c8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="858c8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "798e520d-520d-798e-0d52-8e790d528e79",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```



