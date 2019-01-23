---
title: GroupPolicyPresentationCheckBox を更新します。
description: GroupPolicyPresentationCheckBox オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4150e662109b9dc9d0ebee6a66be12ad1c2473bc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430443"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="e38aa-103">GroupPolicyPresentationCheckBox を更新します。</span><span class="sxs-lookup"><span data-stu-id="e38aa-103">Update groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="e38aa-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e38aa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e38aa-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e38aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e38aa-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e38aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e38aa-107">[GroupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e38aa-107">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e38aa-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e38aa-108">Prerequisites</span></span>
<span data-ttu-id="e38aa-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e38aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e38aa-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e38aa-111">Permission type</span></span>|<span data-ttu-id="e38aa-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e38aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e38aa-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e38aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e38aa-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e38aa-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e38aa-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e38aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e38aa-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e38aa-116">Not supported.</span></span>|
|<span data-ttu-id="e38aa-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e38aa-117">Application</span></span>|<span data-ttu-id="e38aa-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e38aa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e38aa-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e38aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="e38aa-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e38aa-120">Request headers</span></span>
|<span data-ttu-id="e38aa-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e38aa-121">Header</span></span>|<span data-ttu-id="e38aa-122">値</span><span class="sxs-lookup"><span data-stu-id="e38aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e38aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e38aa-123">Authorization</span></span>|<span data-ttu-id="e38aa-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e38aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e38aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e38aa-125">Accept</span></span>|<span data-ttu-id="e38aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e38aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e38aa-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e38aa-127">Request body</span></span>
<span data-ttu-id="e38aa-128">要求の本文に[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="e38aa-128">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="e38aa-129">[GroupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="e38aa-129">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="e38aa-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e38aa-130">Property</span></span>|<span data-ttu-id="e38aa-131">型</span><span class="sxs-lookup"><span data-stu-id="e38aa-131">Type</span></span>|<span data-ttu-id="e38aa-132">説明</span><span class="sxs-lookup"><span data-stu-id="e38aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e38aa-133">label</span><span class="sxs-lookup"><span data-stu-id="e38aa-133">label</span></span>|<span data-ttu-id="e38aa-134">String</span><span class="sxs-lookup"><span data-stu-id="e38aa-134">String</span></span>|<span data-ttu-id="e38aa-135">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="e38aa-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="e38aa-136">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="e38aa-136">The default value is empty.</span></span> <span data-ttu-id="e38aa-137">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e38aa-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e38aa-138">id</span><span class="sxs-lookup"><span data-stu-id="e38aa-138">id</span></span>|<span data-ttu-id="e38aa-139">String</span><span class="sxs-lookup"><span data-stu-id="e38aa-139">String</span></span>|<span data-ttu-id="e38aa-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e38aa-140">Key of the entity.</span></span> <span data-ttu-id="e38aa-141">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e38aa-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e38aa-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e38aa-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e38aa-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e38aa-143">DateTimeOffset</span></span>|<span data-ttu-id="e38aa-144">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="e38aa-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="e38aa-145">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="e38aa-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e38aa-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="e38aa-146">defaultChecked</span></span>|<span data-ttu-id="e38aa-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="e38aa-147">Boolean</span></span>|<span data-ttu-id="e38aa-148">チェック ボックスの既定値です。</span><span class="sxs-lookup"><span data-stu-id="e38aa-148">Default value for the check box.</span></span> <span data-ttu-id="e38aa-149">既定値は、false を指定します。</span><span class="sxs-lookup"><span data-stu-id="e38aa-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="e38aa-150">応答</span><span class="sxs-lookup"><span data-stu-id="e38aa-150">Response</span></span>
<span data-ttu-id="e38aa-151">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e38aa-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e38aa-152">例</span><span class="sxs-lookup"><span data-stu-id="e38aa-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="e38aa-153">要求</span><span class="sxs-lookup"><span data-stu-id="e38aa-153">Request</span></span>
<span data-ttu-id="e38aa-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e38aa-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="e38aa-155">応答</span><span class="sxs-lookup"><span data-stu-id="e38aa-155">Response</span></span>
<span data-ttu-id="e38aa-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e38aa-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "id": "7748190f-190f-7748-0f19-48770f194877",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultChecked": true
}
```




