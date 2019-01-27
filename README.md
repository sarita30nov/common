How to pass  default pros data in child component in react js
TableRow is child component   with withRouter

import { withRouter } from 'react-router-dom';


class TableRow extends Component {

constructor(props) {
        super(props);
    }
    delete() {
        
			this.props.history.push('/index'); // now this will work 
    }

render() {
	  
    return (
        <tr>
          <td>
            {this.props.obj.person_name}
          </td>
</tr>
    );
  }
}
export default withRouter(TableRow);

