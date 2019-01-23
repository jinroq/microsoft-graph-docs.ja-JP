---
title: GroupPolicyPresentationTextBox を更新します。
description: GroupPolicyPresentationTextBox オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 48417f8d3dcc057e535adcf429cc96922c24162a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431599"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="87531-103">GroupPolicyPresentationTextBox を更新します。</span><span class="sxs-lookup"><span data-stu-id="87531-103">Update groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="87531-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="87531-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="87531-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87531-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87531-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="87531-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87531-107">[GroupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="87531-107">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87531-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="87531-108">Prerequisites</span></span>
<span data-ttu-id="87531-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87531-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87531-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87531-111">Permission type</span></span>|<span data-ttu-id="87531-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="87531-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87531-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87531-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87531-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87531-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="87531-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87531-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87531-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87531-116">Not supported.</span></span>|
|<span data-ttu-id="87531-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87531-117">Application</span></span>|<span data-ttu-id="87531-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87531-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87531-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87531-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="87531-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87531-120">Request headers</span></span>
|<span data-ttu-id="87531-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87531-121">Header</span></span>|<span data-ttu-id="87531-122">値</span><span class="sxs-lookup"><span data-stu-id="87531-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87531-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87531-123">Authorization</span></span>|<span data-ttu-id="87531-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="87531-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87531-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87531-125">Accept</span></span>|<span data-ttu-id="87531-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87531-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87531-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="87531-127">Request body</span></span>
<span data-ttu-id="87531-128">要求の本文に[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="87531-128">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="87531-129">[GroupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="87531-129">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="87531-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87531-130">Property</span></span>|<span data-ttu-id="87531-131">型</span><span class="sxs-lookup"><span data-stu-id="87531-131">Type</span></span>|<span data-ttu-id="87531-132">説明</span><span class="sxs-lookup"><span data-stu-id="87531-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87531-133">label</span><span class="sxs-lookup"><span data-stu-id="87531-133">label</span></span>|<span data-ttu-id="87531-134">String</span><span class="sxs-lookup"><span data-stu-id="87531-134">String</span></span>|<span data-ttu-id="87531-135">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="87531-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="87531-136">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="87531-136">The default value is empty.</span></span> <span data-ttu-id="87531-137">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="87531-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="87531-138">id</span><span class="sxs-lookup"><span data-stu-id="87531-138">id</span></span>|<span data-ttu-id="87531-139">String</span><span class="sxs-lookup"><span data-stu-id="87531-139">String</span></span>|<span data-ttu-id="87531-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="87531-140">Key of the entity.</span></span> <span data-ttu-id="87531-141">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="87531-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="87531-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87531-142">lastModifiedDateTime</span></span>|<span data-ttu-id="87531-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87531-143">DateTimeOffset</span></span>|<span data-ttu-id="87531-144">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="87531-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="87531-145">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="87531-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="87531-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="87531-146">defaultValue</span></span>|<span data-ttu-id="87531-147">文字列</span><span class="sxs-lookup"><span data-stu-id="87531-147">String</span></span>|<span data-ttu-id="87531-148">テキスト ボックスに表示される既定の文字列をローカライズします。</span><span class="sxs-lookup"><span data-stu-id="87531-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="87531-149">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="87531-149">The default value is empty.</span></span>|
|<span data-ttu-id="87531-150">必須</span><span class="sxs-lookup"><span data-stu-id="87531-150">required</span></span>|<span data-ttu-id="87531-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="87531-151">Boolean</span></span>|<span data-ttu-id="87531-152">テキスト ボックスに値を入力するための要件。</span><span class="sxs-lookup"><span data-stu-id="87531-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="87531-153">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="87531-153">Default value is false.</span></span>|
|<span data-ttu-id="87531-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="87531-154">maxLength</span></span>|<span data-ttu-id="87531-155">Int64</span><span class="sxs-lookup"><span data-stu-id="87531-155">Int64</span></span>|<span data-ttu-id="87531-156">テキスト文字の最大数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="87531-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="87531-157">1023 を既定値には。</span><span class="sxs-lookup"><span data-stu-id="87531-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="87531-158">応答</span><span class="sxs-lookup"><span data-stu-id="87531-158">Response</span></span>
<span data-ttu-id="87531-159">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="87531-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87531-160">例</span><span class="sxs-lookup"><span data-stu-id="87531-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="87531-161">要求</span><span class="sxs-lookup"><span data-stu-id="87531-161">Request</span></span>
<span data-ttu-id="87531-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87531-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="87531-163">応答</span><span class="sxs-lookup"><span data-stu-id="87531-163">Response</span></span>
<span data-ttu-id="87531-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87531-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```




