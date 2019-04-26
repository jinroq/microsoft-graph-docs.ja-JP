---
title: Azure AD アクセス レビュー
description: Azure AD access レビューを使用して、ユーザーのアクセス権の構成に対して1回限りまたは定期的なアクセスレビューを構成できます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 31b55697601e78fbf1e4af460d1ee7739b126d32
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339217"
---
# <a name="azure-ad-access-reviews"></a>Azure AD アクセス レビュー

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Azure AD access レビュー](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview)を使用して、ユーザーのアクセス権の構成に対して1回限りまたは定期的なアクセスレビューを構成できます。

グループメンバーシップとアプリケーションアクセスのアクセスレビューに関する一般的なお客様のシナリオは、次のとおりです。
   
- お客様は、アクセスレビューを使用して、アプリケーションおよびグループのメンバーシップへのアクセスに関するレビューを使用して、ゲストユーザーのアクセスを確認し、証明できます。 レビュー担当者は、提供された洞察を使用して、ゲストのアクセスを継続する必要があるかどうかを効率的に決定できます。
      
- お客様は、アクセスレビューを使用して、アプリケーションおよびグループメンバーシップへの従業員のアクセスを確認し、証明することができます。
   
- お客様は、コンプライアンスまたはリスクに敏感なアプリケーションのレビューを追跡するために、組織が関連するプログラムにアクセスレビューコントロールを収集できます。

また、グローバル管理者または azure サブスクリプションの役割などの azure AD の役割に割り当てられている管理ユーザーの役割割り当てを確認し、証明するための関連機能もあります。  この機能は、 [Azure AD Privileged Identity Management](privilegedidentitymanagement-root.md)に含まれています。

アクセスレビュー機能 (API を含む) は Azure AD Premium P2 に含まれていることに注意してください。  アクセスレビューを作成するテナントには、有効な、購入済みまたは試用版の Azure AD プレミアム P2 または EMS E5 サブスクリプションが必要です。 アクセスレビュー、プログラム、またはプログラムの制御を作成する前に、管理者は、利用を事前[](programcontroltype.md)に設定し[](businessflowtemplate.md)ておく必要があります。 azure ad のアクセスレビューに、または azure ad の役割または azure サブスクリプションの役割のアクセスレビューの場合は azure ad PIM に、組織をオンボードにすることができます。


## <a name="methods"></a>メソッド 

次の表に、アクセスレビュー関連のリソースを操作するために使用できるメソッドを示します。

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[accessreview を取得する](../api/accessreview-get.md) |   [accessreview](accessreview.md) |   特定の ID を持つアクセスレビューを取得します。 |
|[accessreview を作成する](../api/accessreview-create.md) | [accessreview](accessreview.md) |   新しい accessreview を作成します。 |
|[accessreview の削除](../api/accessreview-delete.md) | なし。   | accessreview を削除します。 |
|[accessreview を更新する](../api/accessreview-update.md) | [accessreview](accessreview.md) | accessreview を更新します。 |
|[accessreview レビュー担当者のリスト](../api/accessreview-listreviewers.md) |      [useridentity](useridentity.md)コレクション| accessreview のレビュー担当者を取得します。 |
|[accessreview レビュー担当者を追加する](../api/accessreview-addreviewer.md) |      なし。   |   閲覧者を accessreview に追加します。 |
|[accessreview レビュー担当者を削除する](../api/accessreview-removereviewer.md) | なし。  |   accessreview からレビュー担当者を削除します。 |
|[accessreview に関する決定事項を一覧表示する](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)コレクション| accessreview の決定事項を取得します。|
|[自分の accessreview の決定事項を一覧表示する](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)コレクション| レビュー担当者として、accessreview の決定事項を取得します。|
|[access レビュー通知の送信](../api/accessreview-sendreminder.md) |        なし。   |   accessreview のレビュー担当者に通知を送信します。 |
|[accessreview を停止する](../api/accessreview-stop.md) |     なし。   |   accessreview を停止します。 |
|[accessreview の決定をリセットする](../api/accessreview-reset.md) |     なし。   |   進行中の accessreview で意思決定をリセットします。|
|[accessreview の決定を適用する](../api/accessreview-apply.md) |     なし。   |   完了した accessreview から決定を適用します。|
|[businessflowtemplates を一覧表示する](../api/businessflowtemplate-list.md) | [businessflowtemplate](businessflowtemplate.md)コレクション| レビューにアクセスするための適切なビジネスフローテンプレートを取得します。|
|[プログラムを作成する](../api/program-create.md) |   [アプリケーション](program.md)   |   新しいプログラムを作成します。|
|[プログラムの削除](../api/program-delete.md) |   なし。   |   プログラムを削除します。|
|[プログラムの一覧表示](../api/program-list.md) |  [プログラム](program.md)コレクション|   すべてのプログラムのコレクションを取得します。|
|[プログラムの programcontrols を一覧表示する](../api/program-listcontrols.md) |      [programcontrol](programcontrol.md)コレクション| プログラムのコントロールのコレクションを取得します。|
|[プログラムの更新](../api/program-update.md) |   [アプリケーション](program.md)|  プログラムを更新します。|
|[programcontrol を作成する](../api/programcontrol-create.md) |     [programcontrol](programcontrol.md) |   プログラムに programcontrol を追加します。|
|[programcontrol の削除](../api/programcontrol-delete.md) |     なし。   |   プログラムから programcontrol を削除します。|
|[programcontrols のリスト](../api/programcontrol-list.md) | [programcontrol](programcontrol.md)コレクション| テナント内のすべてのプログラムでコントロールを一覧表示します。|
|[programcontroltypes のリスト](../api/programcontroltype-list.md) | [programcontroltype](programcontroltype.md)コレクション| プログラムコントロールの種類を一覧表示します。 |

## <a name="role-and-application-permission-authorization-checks"></a>役割とアプリケーションのアクセス許可の承認チェック

呼び出し元ユーザーがアクセスレビュー、プログラム、および制御を管理するには、次のディレクトリの役割が必要です。

| ターゲットリソース | 操作 | アプリケーションのアクセス許可 | 呼び出し元ユーザーの必要なディレクトリの役割 |
|:----------------|:------------------|:------------|:--------------------------------------------|
|Azure AD ロールの[accessreview](accessreview.md) | 読み取り | accessreview を参照してください。すべてのまたは accessreview. | 全体管理者、セキュリティ管理者、セキュリティリーダ、または特権ロール管理者 |
|Azure AD ロールの[accessreview](accessreview.md) | 作成、更新、または削除 | accessreview すべて | グローバル管理者または特権ロール管理者 |
|グループまたはアプリの[accessreview](accessreview.md) | 読み取り | accessreview を参照してください。すべてのまたは accessreview. | グローバル管理者、セキュリティ管理者、セキュリティリーダ、またはユーザー管理者 |
|グループまたはアプリの[accessreview](accessreview.md) | 作成、更新、または削除 | accessreview すべて | 全体管理者またはユーザー管理者 |
| [プログラム](program.md)および[programcontrol](programcontrol.md)| 読み取り | programcontrol. すべてのまたはすべてのプログラムを読み取ることができます。 |  グローバル管理者、セキュリティ管理者、セキュリティリーダ、またはユーザー管理者 |
| [プログラム](program.md)および[programcontrol](programcontrol.md) | 作成、更新、または削除 | programcontrol | 全体管理者またはユーザー管理者 |

また、アクセスレビューの担当者に割り当てられているユーザーは、ディレクトリロールに存在しなくても、決定を管理できます。

## <a name="see-also"></a>関連項目

- [管理者が Azure AD アクセスレビューを使用してユーザーアクセスを管理する方法](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [管理者が Azure AD アクセスレビューでゲストアクセスを管理する方法](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [管理者が Azure AD アクセスレビューのプログラムとコントロールを管理する方法](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
